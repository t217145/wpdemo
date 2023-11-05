How to use
---
Prerequisite
+ Create an Azure account
+ Cloud shell is ready

Before run
---
After git clone this repo, <span style='color: red;'><b>change the MySQL password in <u>docker-compose.yml</u> file</b>.</span>

Code to run
---
```
git clone https://github.com/t217145/wpdemo.git
cd wpdemo
terraform init
terraform plan -out main.tfplan
terraform apply main.tfplan
$default_site_hostname = terraform output --raw default_site_hostname
echo $default_site_hostname
```