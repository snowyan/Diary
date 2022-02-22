### 1.how to make a mp4 video, 
* refrence /snow/Documents/ml/Notes/make_video.ipynb
### 2.how to connect the path in python
* refrence the following example
* epoch = 10
* checkpoint_dir = '/model'
* checkpoint_path = '/model/{}/'.format(epoch)
### 3.how to remove databricks folder
* notes the path does not include /dbfs
* dbutils.fs.rm(("/snow/MNISTDemo/train"), recurse=True)
### How to know how many cores in mac
* "About this mac"->"System Report"->"Hardware"->"Hardware Overview"
