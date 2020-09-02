macOS - macOS Bootstrap Playbook
================================

On a new machine, run:

```bash
xcode-select --install

curl "https://bootstrap.pypa.io/get-pip.py" -o /tmp/get-pip.py
sudo python /tmp/get-pip.py
sudo pip install ansible
export PYTHONUNBUFFERED=1
export PYTHONIOENCODING='utf-8'
ansible-pull -K -d /tmp/bootstrap -i localhost, -e 'ansible_python_interpreter=/usr/bin/python3' -U https://github.com/jalaziz/macos.git
```

