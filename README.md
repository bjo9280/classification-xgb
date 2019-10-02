# cls_exam

https://github.com/tensorflow/models/tree/master/research/slim

### Pretrained model

<https://github.com/tensorflow/models/tree/master/research/slim#Pretrained> 

### Training a model from scratch.

```
python ../slim/train_image_classifier.py
 --train_dir save
 --dataset_dir tfrecords
 --dataset_split_name train
 --model_name resnet_v2_101
 --checkpoint_path checkpoints/resnet_v2_101.ckpt
 --depth_multiplier 1.0
 --train_image_size 224
 --max_number_of_steps 1000
 --save_summaries_secs 30
 --save_interval_secs 300
 --dataset_name custom
 --dataset_num_classes 9
 --dataset_num_train_samples 356
 --dataset_num_validataion_samples 92
 --log_every_n_steps 20
 --fast_mode True
 --optimizer momentum
 --batch_size 32
 --learning_rate 0.001
 --end_learning_rate 1e-05
 --learning_rate_decay_factor 0.94
 --checkpoint_exclude_scopes resnet_v2_101/logits,resnet_v2_101/SpatialSqueeze,resnet_v2_101/predictions
 --preprocessing_name resnet_v2_101
```

