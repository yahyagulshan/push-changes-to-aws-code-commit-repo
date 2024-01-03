# push-changes-to-aws-code-commit-repo

* login to the AWS console
* open the AWS CodeCommit
* and copy the url from there
* open your terminal and paste the below command for clone the repo on local

`git clone https://git-codecommit.us-east-1.amazonaws.com/v1/repos/video-repo`
# Create username and password for aws-code-commit

* for cloning the repo on localy it will ask the username and password 
* Open IAM user and go to security credentials
* Drop down the page and go to HTTPS Git credentials for AWS CodeCommit (1)

![Screenshot from 2024-01-03 18-32-15](https://github.com/yahyagulshan/push-changes-to-aws-code-commit-repo/assets/59036269/7467bac6-65f8-4485-8561-e48eeede641a)


* Here click generate credentials.

* AWS provides us with username and password information to use the AWS code commit repository.

* Now use the below commands for push changes on the aws code commit.

* cd into that directory first

`git config --local user.name "yahya-admin-at-960742198541"`

`git config --local user.email yahyaaawan4246@gmail.com`

`git config --local init.defaultBranch main`

`git add test.tf`

`git commit -m "add new file test.tf"`

`git push origin main`

Now we again give the username and password and our changes will push to the aws code commit repository.
