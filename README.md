# travis-ubuntu-systray
systray icon for travis for ubuntu

Note: this isnt currently quite really working for now.

- first copy travis.yaml.templ to travis.yaml
- customize to contain a github apikey, with permissions:
  - repo:status
  - repo_deployment
  - public_repo
  - user:email
- put list of repos to watch, in format `your_username/repo_name`
- install python3.5, as virtualenv
- activate the virtualenv, then do:
```
pushd $VIRTUAL_ENV/lib/python3.5/site-packages
ln -s /usr/lib/python3/dist-packages/gi/ .
popd
pip install travispy
```
- `pip install travispy`
- run like `python travis_systray.py`

<img src="img/travis_systray.png?raw=true" />
