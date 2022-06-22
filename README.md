# Ansible Laptop Configuration

Configuration for my Ubuntu Laptop (tested on Ubuntu 22.04)

The Ansible playbook `playbook.yml` contains serval tasks (i.e. the Ansible unit of action) grouped by roles

- Download / git clone this repo
- Install Ansible
```shell
sudo apt update
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```

- Install the roles from [Ansible Galaxy](https://galaxy.ansible.com/home)
```shell
ansible-galaxy install -r requirements.yml
```

- Install all the things (you will need to type your sudo password once).
```sh
ansible-playbook playbook.yml -K
```

## Credits

- [Benoth/ansible-ubuntu](https://github.com/Benoth/ansible-ubuntu)
- [jackdbd/ansible-laptop](https://github.com/jackdbd/ansible-laptop)
