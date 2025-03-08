# lab9
Firstly install aws, packer, and terraform using the instructions in these notes:
https://gitlab.com/cit_4640/4640-notes-w25 

Next generate an ssh key pair:
ssh-keygen -t ed25519 -f </name/of/key>

Next run the import key script to upload the keys to aws. 

Going into packer now, you will first initialize the packer directory and check the format of the main.tf file with:
packer init .
packer validate .

Then build with:
packer build .

Lastly for terraform, intialize the directory and validate the terrafrom files with:
terraform init 
terraform validate

And finally, to apply the file:
terraform apply -auto-approve

To destroy all the resources used with terraform, use the command:
terraform destroy
