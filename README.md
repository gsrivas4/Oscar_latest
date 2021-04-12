# Oscar: Object-Semantics Aligned Pre-training for Vision-and-Language Tasks    <img src="docs/oscar_logo.png" width="200" align="right"> 

* `git clone https://github.com/gsrivas4/Oscar_latest`
* cd Oscar_latest
* `git clone https://github.com/huggingface/transformers`
* cd transformers
* `git checkout 067923d3267325f525f4e46f357360c191ba562e`
* `cd ..`
* `mkdir pretrained_models`
* `cd pretrained_models`
* `wget https://biglmdiag.blob.core.windows.net/oscar/pretrained_models/base-vg-labels.zip`
* `unzip base-vg-labels.zip`
* `cd ..`
* Download dataset using the instructions on this link https://github.com/microsoft/Oscar/blob/master/DOWNLOAD.md#note - install azcopy and then run `path/to/azcopy copy https://biglmdiag.blob.core.windows.net/oscar/datasets/coco_caption.zip <local_path>`
* `pip install boto3`

