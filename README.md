# travis-ubuntu-systray
systray icon for travis for ubuntu

- first copy travis.yaml.templ to travis.yaml
- customize to contain a github apikey, with permissions:
  - repo:status
  - repo_deployment
  - public_repo
  - user:email
- put list of repos to watch, in format `your_username/repo_name`
- run like `python travis_systray.py`

<img src="img/travis_systray.png?raw=true" />
