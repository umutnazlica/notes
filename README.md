 🧪 Usefull Commands related to SQLcl,GIT, GH

> 💡 Some usefull commands and notes related to using tools like SQLcl, GIT etc

## 🌟 Additional Resources


## 🌟 SQLcl

Connect without login <br>

```bash
sql /nolog
```
Connect and save with speccifying tns admin path, (modify user, pwd, service name, tnsnames.ora location)

```bash
export TNS_ADMIN=“/home/opc/dbcicd-demo/wallet/dev1”
```
```bash
sql /nolog
```
```bash
connect -save hr_dev1_new -savepwd user/password@myatp_low(servicename)?TNS_ADMIN=“/home/opc/dbcicd-demo/wallet/dev1"
```
list existing connections within sqlcl

```bash
connmgr list
```
connect to an existing connection
```bash
conn -name hr_dev1
```
run a existing sqlscript after connected within sqlcl (modify the path and script name!)

```bash
@/home/opc/dbcicd-demo/scripts/salary_increase_performance.sql
```



