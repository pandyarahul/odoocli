
# Odoo CLI

Daily useful commands for Odoo Developer and GitHub cheat sheet.


## GitHub Cheat Sheet

Clone Odoo
```bash
https://github.com/odoo/odoo.git
```
Clone Odoo Single Branch
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
git add --all
```
Commit 
```bash
git commit -m "Issue Fiexed"
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
git config --global user.email 'hello.rahul@aol.com'
```

Local username & email 
```bash
git config user.name "Jakub Pawlowicz"
git config user.email '<email>'
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
Clone Odoo 
```bash
ssh-keygen -t rsa
```

#### Check & Kill Service 
```bash
ps -ax  |  grep  "odoo"
kill -9  service_no
```
# Odoo CLI
#### Run Odoo using Config File
```bash
python3.7 /home/rahul/workspace/odoo_15/odoo/odoo-bin -c /home/rahul/Downloads/odoo_v15.conf
```

#### Odoo 8.0 
```bash
./openerp-server --addons-path=addons,../custom_addons_8 --xmlrpc-port=8008 --db-filter=v8
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

Clone Odoo 
```bash
sudo python3.8 -m pip install pyopenssl
python3.8 -m pip install PyPDF2==1.26.0
python3.8 -m pip install -r /home/odoo/requirements.txt
sudo python3.8 -m pip install -r requirements.txt
```

### Extend Enterprise Expiry

Clone Odoo 
```bash
web_enterprise > home_menu.js > _enterpriseExpirationCheck()  >         
var dbexpirationDate = new moment(new moment().add(100000, 'd'));
```
```bash
Technical > System Parameters ;
Type in "database.expiration_date"
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
UPDATE rma_main SET state = 'draft' WHERE ID = 8;
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

## Support

For support, email hello.rahul@aol.com 😊
## Authors

- [@pandyarahul](https://github.com/pandyarahul)


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://pandyarahul.odoo.com//)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pandyarahul/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/pandyarahul4u/)

