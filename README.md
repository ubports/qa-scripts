# qa-scripts

A simple python script to test pull-requests on UBports repositories.

## Usage

```
phablet@ubuntu-phablet:~$ ubports-qa
usage: ubports-qa [-h] {install,remove,list,update} ...

UBports QA scripts

positional arguments:
  {install,remove,list,update}
    install             Add pr to install
    remove              Remove installed repo
    list                List installed repos
    update              Update system using apt

optional arguments:
  -h, --help            show this help message and exit
```
