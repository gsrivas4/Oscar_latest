# Oscar: Object-Semantics Aligned Pre-training for Vision-and-Language Tasks    <img src="docs/oscar_logo.png" width="200" align="right"> 

* `git clone https://github.com/gsrivas4/Oscar_latest`
* cd Oscar_latest
* `git clone https://github.com/huggingface/transformers`
* cd transformers
* `git checkout master`
* `pip install trasformers`
* `cd ..`
* `mkdir pretrained_models`
* `cd pretrained_models`
* `wget https://biglmdiag.blob.core.windows.net/oscar/pretrained_models/base-vg-labels.zip`
* `unzip base-vg-labels.zip`
* `cd ..`
* Download dataset using the instructions on this link https://github.com/microsoft/Oscar/blob/master/DOWNLOAD.md#note - install azcopy and then run path/to/azcopy copy https://biglmdiag.blob.core.windows.net/oscar/datasets/coco_caption.zip <local_path>
* `pip install boto3`
* run `python oscar/run_captioning.py --model_name_or_path pretrained_models/base-vg-labels/ep_67_588997 --do_train --do_lower_case --evaluate_during_training --add_od_labels --learning_rate 0.00003 --per_gpu_train_batch_size 64 --num_train_epochs 30 --save_steps 5000 --output_dir output/`

