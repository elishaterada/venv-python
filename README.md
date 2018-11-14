# Virtualenv + direnv setup script

## Summary

Setup Python 3+ development environment in [Virtualenv](https://virtualenv.pypa.io/en/stable/) with the power of [direnv](https://direnv.net/) so you don't have to worry about activating and deactivating anything at all. Just `cd` into and out of your project directories and `direnv` will automatically activate / deactivate your `Virtualenv`.

## Install (Mac OSX)

1. Install `direnv` and `Virtualenv`
2. Create a directory at `~/bin` and move `venv-python` shell script
3. In your `~.bash_profile` add `export PATH="$HOME/bin:$PATH";` so that the above script can be executed in the shell
4. In your `~/.bash_profile` add `eval "$(direnv hook bash)"` so that direnv can kick-in whenever you `cd` into the project directory
5. You can now setup your direnv by simply typing `venv-python` in the desired directory

## Related Repos
* [Django Setup](https://github.com/elishaterada/django-setup) - Quickly scaffold your Django project with shell script.

## Resources
* [Virtualenv](https://virtualenv.pypa.io/en/stable/)
* [direnv](https://direnv.net/)
* [Practical direnv](https://rnorth.org/practical-direnv)
