### Pythoch use
* !stylegan2_pytorch --data /dbfs/FileStore/tables/cloths_hm_GAN_resized --name hm-gen-256 --multi-gpus --aug-prob 0.5 --num-train-steps 2000000 --results_dir /dbfs/aihackathon/we-gan-do-it/hm256/results --models_dir /dbfs/aihackathon/we-gan-do-it/hm256/models --image-size 256

### My working
gan_invest_deom: 

This notebook demonstrates how to construct DGANs and how to train the DGANs model on the two clusters with two GPUs using Multimirror distributed strategy and Horovod strategy.

https://adb-417473346426606.6.azuredatabricks.net/?o=417473346426606#notebook/1302644048745338

DCgans:

This notebook demonstrates how to construct DCGANs in one machine one GPU

https://adb-417473346426606.6.azuredatabricks.net/?o=417473346426606#notebook/1950522072298394

image_data_process:

This notebook demonstrates how to load image data and save the binary data to tf-record format.

https://adb-417473346426606.6.azuredatabricks.net/?o=417473346426606#notebook/3763044440664903

