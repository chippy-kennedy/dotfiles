### Setting Up New Python Env
[borrowed from DO Community](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-macos)
```
cd ~/dir/of/installed-envs/
python3.7 -m venv my_env
```


### Using Python Envs

**Activating Env:**
```
cd ~/dir/of/installed-envs/
source <my_env>/bin/activate
```

**Deactivating Env:**
(from anywhere)
```
deactivate
```

### Notes
- Within the virtual environment, you can use the command python instead of python3, and pip instead of pip3 if you would prefer. If you use Python 3 on your machine outside of an environment, you’ll need to use the python3 and pip3 commands exclusively, as python and pip will call an earlier version of Python.
