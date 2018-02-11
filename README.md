# Terraform on Azure

Prerequisite on linux: azure cli, terraform and git.<br>
Prerequisite on windows: azure cli, terraform, git and powershell/git-bash.

## Follow the instructions below, 

$ az login<br>
Copy the url, paste it on the browser.  then copy the code and paste it on the browser.<br>
This should output the account info, grab the subscription-id and put below.<br>

$ az ad sp create-for-rbac --role="Contributor" --scopes="/subscriptions/subscription-id"<br>
This will output the appid, the password which is the clientsecret and the tenantid.  Put it on the terraform.tfvars.

$ git clone https://github.com/itikabc/terraform.git<br>
$ cd terraform1<br>
$ terraform init<br>
$ terraform plan<br>
$ terraform apply<br>

---do your testing---

$ terraform destroy
 
