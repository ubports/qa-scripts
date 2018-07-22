# qa-scripts

The UBports QA scripts allow you to efficiently manage PPAs from
repo.ubports.com for testing deb components. See
http://docs.ubports.com/en/latest/about/process/ppa.html.

## Usage

```
phablet@ubuntu-phablet:~$ ./ubports-qa
usage: ubports-qa [-h] {install,remove,list,update} ...

The UBports QA scripts allow you to efficiently manage PPAs from
repo.ubports.com for testing deb components. See
http://docs.ubports.com/en/latest/about/process/ppa.html.

positional arguments:
  {install,remove,list,update}
    install             Install a ppa or pull-request
    remove              Remove and uninstall a PPA
    list                List installed PPAs
    update              Update all packages using apt

optional arguments:
  -h, --help            show this help message and exit
```

### Examples

| Command | Explaination |
|---|---|
| `sudo ubports-qa install xenial_-_somebranch` | Add the `xenial_-_somebranch` ppa and install upgrade all packages |
| `sudo ubports-qa install dialer-app 5` | Add the branch of the fifth pull-request on the dialer-app as a PPA and upgrade all packages |
| `sudo ubports-qa remove xenial_-_somebranch` | Remove the `xenial_-_somebranch` ppa and upgrade all packages |
| `ubports-qa list` | List all installed testing-PPAs |
| `sudo ubports-qa update` | Upgrade all packages |
