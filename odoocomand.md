
# 🛠 Odoo CLI

Daily useful commands for Odoo Developer and GitHub cheat sheet.


## GitHub Cheat Sheet

Clone Odoo
```bash
git clone https://github.com/odoo/odoo.git
```
```bash
git clone https://www.github.com/odoo/odoo --depth 1 --branch 12.0 --single-branch
```
Check Status 
```bash
git status
```
Add Commit
```bash
git add *
```
```bash
git add --all
```
Commit 
```bash
git commit -m "Issue Fiexed"
```
```bash
git commit -am "[ADD] Issue Fixed"
```
Push Commit 
```bash
git push
```

List all branches
```bash
git branch -a
```

Create a branch
```bash
git checkout -b <name>
```

Revert commit 
```bash
git revert -n <sha>
```

Reset HEAD to n commits back 
```bash
git reset --hard HEAD~<n>
```

search git log commits 
```bash
git log -S “free text”
```

Global username & email 
```bash
git config --global user.name "Pandya Rahul"
```
```bash
git config --global user.email "hello.rahul@aol.com"
```

Local username & email 
```bash
git config user.name "Pandya Rahul"
```
```bash
git config user.email "hello.rahul@aol.com"
```

Clone Specific Branch 
```bash
git clone git@bitbucket.org:browseinfo/sale_purchase_addons -b 12.0
```

Checkout Specific Branch 
```bash
git fetch && git checkout 12.0
```

Remove File from Repo 
```bash
git rm -r bi_website_dimension
```

Remove Changes from Repo 
```bash
git clean -df
```
#### Generate SHH Key 
```bash
ssh-keygen -t rsa
```
```bash
cat ~/.ssh/id_rsa.pub
```

#### Check & Kill Service 
```bash
ps -ax  |  grep  "odoo"
```
```bash
kill -9  service_no
```
# 🚀 Odoo CLI
#### Run Odoo using Config File
```bash
python3.8 /home/rahul/workspace/odoo_15/odoo/odoo-bin -c /home/rahul/Downloads/odoo_v15.conf
```
#### Config File
```bash
[options]
addons_path = /home/rahul/workspace/odoo_15/odoo,/home/rahul/workspace/odoo_15/odoo/odoo,/home/rahul/workspace/odoo_15/custom_addons_15
admin_passwd = admin_123
db_host = localhost
db_password = odoo
db_port = 8015
db_user = odoo
http_port = 8015
;dbfilter = 
limit_time_real = 1200000
```

#### Odoo 8.0 
```bash
python2.7 ./openerp-server --addons-path=addons,../custom_addons_8 --xmlrpc-port=8008 --db-filter=v8
```

#### Odoo 9.0
```bash
python2.7 ./openerp-server --addons-path=addons,../custom_addons_9 --xmlrpc-port=8009 --db-filter=v9
```

#### Odoo 10.0
```bash
./odoo-bin --addons-path=addons,../custom_addons_10 --dev=reload --xmlrpc-port=8010 --db-filter=v10
```
#### Odoo 11.0

#### Community Edition
```bash
python3.6 odoo-bin --addons-path=addons,../custom_addons_11 --xmlrpc-port=8011 --db-filter=v11
```
#### Enterprise Edition
```bash
python3.6 ./odoo-bin --addons-path=odoo/addons,../custom_addons_11e --xmlrpc-port=8021 --db-filter=v11e
```

#### Odoo 12.0

#### Community Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_11 --xmlrpc-port=8011 --db-filter=v11
```
#### Enterprise Edition
```bash
python3.8 ./odoo-bin --addons-path=odoo/addons,../custom_addons_12e --xmlrpc-port=8022 --db-filter=v12e
```
#### Odoo 13.0

#### Community Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_13 --xmlrpc-port=8013 --db-filter=v13
```
#### Enterprise Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_13e --xmlrpc-port=8023 --db-filter=v13e
```
#### Odoo 14.0

#### Community Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_14 --xmlrpc-port=8014 --db-filter=v14
```
#### Enterprise Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_14e --xmlrpc-port=8024 --db-filter=v14e
```

#### Odoo 15.0

#### Community Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_15 --xmlrpc-port=8015 --db-filter=v15
```
#### Enterprise Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_15e --xmlrpc-port=8025 --db-filter=v15e
```

#### Odoo 16.0

#### Community Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_16 --xmlrpc-port=8016 --db-filter=v16
```
#### Enterprise Edition
```bash
python3.8 odoo-bin --addons-path=addons,../custom_addons_16e --xmlrpc-port=8026 --db-filter=v16e
```

### Python Useful Commands 
```bash
sudo python3.8 -m pip install pyopenssl
```
```bash
python3.8 -m pip install PyPDF2==1.26.0
```
```bash
python3.8 -m pip install -r /home/odoo/requirements.txt
```
```bash
sudo python3.8 -m pip install -r requirements.txt
```
Install Python for Specific Version 
```bash
sudo apt-get upgrade
```
```bash
sudo add-apt-repository ppa:deadsnakes/ppa
```
```bash
sudo apt-get update
```
```bash
sudo apt-get install python3.5
```

Install Python with Specific Packages 
```bash
sudo apt install python3.8-dev
```
```bash
sudo apt install python3.8-venv
```
```bash
sudo apt install python3.8-distutils
```
```bash
sudo apt install python3.8-tk
```

Remove Python 
```bash
sudo apt-get remove python3*
```

### Extend Enterprise Expiry

```bash
web_enterprise > home_menu.js > _enterpriseExpirationCheck()  >         
var dbexpirationDate = new moment(new moment().add(100000, 'd'));
```
```bash
Setting > Technical > System Parameters ;
Type in "database.expiration_date"
```
```bash
psql db_name;
select id,key from ir_config_parameter;
UPDATE ir_config_parameter SET value='2091-04-05 11:13:05' WHERE ID =23;
```

## PostgreSQL Commands

Start PostgreSQL 
```bash
psql database_name
```

Show Availble Databse 
```bash
\l
```
Enter into Databse 
```bash
\c
```
Show Available Tables in Database 
```bash
\dt *.*
```

Show Columns of Table 
```bash
\d
```
List Databse Users 
```bash
\du
```
Select Databse User
```bash
\SELECT current_user;
```
Delete Query 
```bash
delete from account_move where id=11;
```
Update Query 
```bash
UPDATE invoice_sale_commission SET readonly = False WHERE ID = 1;
```
```bash
UPDATE rma_main SET state = 'draft' WHERE ID = 8;
```
```bash
UPDATE res_users SET login = 'admin' WHERE ID = 2;
```
Exit 
```bash
\q
Ctrl + D
```
Restart PostgreSQL Service 
```bash
sudo service postgresql restart
```

#### Restore Database from SQL 
```bash
sudo su postgres
```
```bash
psql
```
```bash
createdb -U postgres databse_name
```
```bash
psql -U postgres -d databse_name -f /home/rahul/[path]/dump.sql
```
```bash
ALTER DATABASE databse_name OWNER TO ubantu_user;
```

## Support

For support, email hello.rahul@aol.com 😊

## Authors

- [@pandyarahul](https://github.com/pandyarahul)


## 🔗 Socials
[![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white)](https://facebook.com/pandyarahul4u) 
[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=Twitter&logoColor=white)](https://twitter.com/pandyarahul4u)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/pandyarahul4u)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/pandyarahul) 
[![Pinterest](https://img.shields.io/badge/Pinterest-%23E60023.svg?logo=Pinterest&logoColor=white)](https://pinterest.com/pandyarahul4u) 
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?logo=YouTube&logoColor=white)](https://youtube.com/@pandyarahul) 
[![Stack Overflow](https://img.shields.io/badge/-Stackoverflow-FE7A16?logo=stack-overflow&logoColor=white)](https://stackoverflow.com/users/17455752)

[![GitHub WidgetBox](https://github-widgetbox.vercel.app/api/profile?username=pandyarahul&data=followers,repositories,stars,commits&theme=nautilus)](https://github.com/Jurredr/github-widgetbox)

<h2 align="center">Value my work? Fuel my motivation with a cup of coffee! ☕</h2>
<p align="center">
	<a align="center" href="https://www.buymeacoffee.com/pandyarahul"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=pandyarahul&button_colour=FF5F5F&font_colour=ffffff&font_family=Arial&outline_colour=000000&coffee_colour=FFDD00" /></a>
</p>
