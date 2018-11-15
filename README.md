# Tentacle

```
.___________. _______ .__   __. .___________.    ___       ______  __       _______
|           ||   ____||  \ |  | |           |   /   \     /      ||  |     |   ____|{0.1.0#test}
`---|  |----`|  |__   |   \|  | `---|  |----`  /  ^  \   |  ,----'|  |     |  |__
    |  |     |   __|  |  . `  |     |  |      /  /_\  \  |  |     |  |     |   __|
    |  |     |  |____ |  |\   |     |  |     /  _____  \ |  `----.|  `----.|  |____
    |__|     |_______||__| \__|     |__|    /__/     \__\ \______||_______||_______| http://www.orleven.com


```

Just for pentest.

[![Python 3.5](https://img.shields.io/badge/python-3.5-yellow.svg)](https://www.python.org/)

![show](https://raw.githubusercontent.com/orleven/tentacle/master/show/test.png)

### Usage

```
# Show help for tentacle.
py -3 tentacle.py --help

# Show all modual, and you can see it in `script` path.
py -3 tentacle.py -n --show

# Load modual by -m (e.g. web_status,@web)
py -3 tentacle.py -n -m web_status # Load web_status modul
py -3 tentacle.py -n -m @web # Load all module of web path
py -3 tentacle.py -n -m web_status,@web # Load all module of web path and web_statusmodule
py -3 tentacle.py -n -m * # Load all module

# Load target by iS/iN/iF/iT.
py -3 tentacle.py -n -m web_status -iS www.examples.com -iN 192.168.111.0/24
py -3 tentacle.py -n -m web_status -iN 192.168.111.0/24
py -3 tentacle.py -n -m web_status -iF target.txt
py -3 tentacle.py -n -m web_status -iT dcc54c3e1cc2c2e1 # Load task by recode's target

# Show all function of module by -f show or -f help
py -3 tentacle.py -n -m web_status -f show
py -3 tentacle.py -n -m web_status -f help

# Use function of modual by -m and -f  (e.g. -m web_status -f prove), and you should make sure the function of module is exist.
py -3 tentacle.py -n -m web_status -f prove

# Show task' result by -tS
py -3 tentacle.py -n -tS 8d4b37597aaec25e

# Export task' result by -tS to test.xlsx
py -3 tentacle.py -n -tS 8d4b37597aaec25e  -o test
```

### Update

[2018-11-15] code refactoring and fix nomal model's bug.

### Coming

1. scan timeout bug
2. struts2 mixtake bug
3. crawler module
4. log color
5. module(script) clean up
6. server model
7. client model
8. someone gbk code and log bug
9. update
10. config(proxy...)
11. port scan
12. and...


### Thanks

1. Sqlmap
2. POC-T
