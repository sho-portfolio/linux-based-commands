# python-cheatsheet

# Install sudo
```pip install sudo```
```pip install --upgrade --user pip```

# Install Pip on debian
https://linuxize.com/post/how-to-install-pip-on-debian-9/
</br>```sudo apt update```
</br>```sudo apt install python-pip```

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
''''
(wget is not installed on mac os by default, but curl is and it's similar)
