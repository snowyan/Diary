### how to make a mp4 video, 
* refrence /snow/Documents/ml/Notes/make_video.ipynb
### how to connect the path in python
* refrence the following example
* epoch = 10
* checkpoint_dir = '/model'
* checkpoint_path = '/model/{}/'.format(epoch)
### how to remove databricks folder
* notes the path does not include /dbfs
* dbutils.fs.rm(("/snow/MNISTDemo/train"), recurse=True)
