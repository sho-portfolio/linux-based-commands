# python-cheatsheet

# Install PIP
https://pip.pypa.io/en/stable/installing/


# Install Python on a new machine (and virtual environments)
https://wsvincent.com/install-python3-mac/

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
