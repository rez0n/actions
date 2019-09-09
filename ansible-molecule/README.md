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
* ubuntu1604
* ubuntu180
* ubuntu1404
* ubuntu1204
* debian10
* debian9
* debian8
* centos7
* centos6
* amazonlinux2
* fedora30
* fedora29
* fedora27
* fedora24
* ubi8

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