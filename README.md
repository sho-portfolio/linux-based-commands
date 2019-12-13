# python-cheatsheet

# Install sudo
<br/>```pip install sudo```
<br/>```pip install --upgrade --user pip```

# Install Pip on debian
https://linuxize.com/post/how-to-install-pip-on-debian-9/
</br>```sudo apt update```
</br>```sudo apt install python-pip```

# Install Pip on Amazon Linux based AMI
https://linuxize.com/post/how-to-install-pip-on-debian-9/
</br>```sudo yum update```
</br>```sudo yum install python-pip```
</br> * NOTE: replace apt-get with yum as Amazon Linux based AMI uses the yum command instead of apt-get
</br> * NOTE: On Debian derivatives such as Ubuntu, use apt. 
</br> * NOTE: On Red Hat and derivatives, use yum. 
</br> * NOTE: On SUSE and derivatives, use zypper
</br> * [https://docs.aws.amazon.com/cli/latest/userguide/install-linux-python.html]


# Install PIP
https://pip.pypa.io/en/stable/installing/
[Note that when you run the second command be sure to add --user if you get an error eg: python get-pip.py --user]

# Install Python on a new machine (and virtual environments)
https://wsvincent.com/install-python3-mac/
<br/>```xcode-select --install```
<br/>```/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```
<br/>```brew install python3```
<br/>
<br/>
<br/>


# Install tensorflow on Debian
```pip3 install --upgrade tensorflow```
(on aws) If you get an MemoryError or a Permission error try this: 
```pip install --no-cache-dir --user tensorflow```


# Install Jupyter
https://jupyter.org/install



# Read Excel file
!pip install -q xlrd
import pandas as pd
df = pd.read_excel('courses/deeplearning1/excel/layers_example.xlsx')
print(df)


# Install Google SDK (if you want to use it)
https://cloud.google.com/sdk/docs/quickstart-macos

# How to connect Colab to a VM (Compute Engine)
https://medium.com/@senthilnathangautham/colab-gcp-compute-how-to-link-them-together-98747e8d940e
* did not work

# use datalab instead
https://cloud.google.com/datalab/docs/quickstart
*this works

in the datalab notebook you need to:
open all the files from icloud into datalab
!pip install --upgrade tensorflow
!pip install keras
then run main.py

# try this to integrate with github (see the second comment)
https://stackoverflow.com/questions/43467217/how-to-pull-and-push-notebooks-to-github-from-google-cloud-datalab

# copy files from google buckets to google vm
https://cloud.google.com/storage/docs/quickstart-gsutil#create
## list bucket files from vm
gsutil ls gs://my-awesome-bucket
## copy from bucket to vm
gsutil cp gs://my-awesome-bucket/file1.png file1.png
gsutil cp gs://my-awesome-bucket/file1.png Desktop/file1.png

# Make file on google bucket accessible to everyone
gsutil acl ch -u AllUsers:R gs://my-awesome-bucket/file1.png


# install git on VM (Debian9)
https://www.digitalocean.com/community/tutorials/how-to-install-git-on-debian-9
```
sudo apt update
sudo apt install git
```


# copy/clone from github to vm
```
git clone https://github.com/sho-portfolio/MachineLearning-MultiClassClassifier.git
ls
```

# Copy single file from Github to VM
https://stackoverflow.com/questions/4604663/download-single-files-from-github
```
wget https://raw.githubusercontent.com/sho-portfolio/MachineLearning-MultiClassClassifier/master/dataTest.txt
```

# install wget on mac
https://www.hacksparrow.com/os/how-to-install-wget-on-your-mac.html
```
brew install wget
```
(wget is not installed on mac os by default, but curl is and it's similar)



# install mysql on EC2 instance
https://medium.com/@chamikakasun/installing-mysql-in-an-ec2-instance-55d6a3e19caf
once you've created an EC2 instance and SSH'd into it
```sudo su```
```yum update -y```
```yum install mysql-server```
```service mysqld start```

to connect to the aws mysql instance you created on rds use this command:

```mysql -h <end-point> -P 3306 -u <user-name> -p```
```mysql -h sho-youtube.c4lxnjkjrvz9.us-east-1.rds.amazonaws.com -P 3306 -u root -p```
[note: you'll need to be sure that the inbound security group allows access from the ec2 ip or some "anywhere"]
