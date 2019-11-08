# python-cheatsheet

# Install Pip on debian
https://linuxize.com/post/how-to-install-pip-on-debian-9/

# Install PIP
https://pip.pypa.io/en/stable/installing/
[Note that when you run the second command be sure to add --user if you get an error eg: python get-pip.py --user]

# Install Python on a new machine (and virtual environments)
https://wsvincent.com/install-python3-mac/


# Install git on debian 9
https://www.digitalocean.com/community/tutorials/how-to-install-git-on-debian-9

# Install tensorflow on Debian
pip3 install --upgrade tensorflow


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

