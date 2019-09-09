## How to use

* Add `action-ansible-molecule.yml` into your's workflows directory `<repo>/.github/workflows/`
* Add molecule tests following `molecule-example`

## Configure
You can choose list of OS images for test your role.
```
        os:
          - centos7
          - ubuntu1804
```
Available OS variants [@geerlingguy Docker Hub](https://hub.docker.com/u/geerlingguy) docker-*-ansible
* docker-ubuntu1604-ansible
* docker-ubuntu1804-ansible
* docker-ubuntu1404-ansible
* docker-ubuntu1204-ansible
* docker-debian10-ansible
* docker-debian9-ansible
* docker-debian8-ansible
* docker-centos7-ansible
* docker-centos6-ansible
* docker-amazonlinux2-ansible
* docker-fedora30-ansible
* docker-fedora29-ansible
* docker-fedora27-ansible
* docker-fedora24-ansible
* docker-ubi8-ansible

And you can choose ANsible versions list to test.
```
        ansible:
          - 2.8
          - 2.7
          - 2.6.*
```
* 2.8 = 2.8.0
* 2.8.* = latest 2.8.
* 2.7.5 = 2.7.5


## Credits

`molecule-example` from @geerlingguy ansible roles.

Docker images used for molecule tests are from @geerlingguy Docker Hub.