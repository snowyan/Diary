### How to select the tf dataset's buffle size
* For perfect shuffling, a buffer size greater than or equal to the full size of the dataset is required.
### How to convert image numpy data to tf dataset
* tf.convert_to_tensor
* tf.data.Dataset.from_tensor_slices
