**Environment:**

 Google collab pro was used to train the models on GPU

**Dataset: **

1. Under Datasets, download all the training, validation, testing as well as face annotations from the below link 

http://shuoyang1213.me/WIDERFACE/

2. CD to the Datasets folder  and convert downloaded wider face dataset into COCO format with the following command

!python face_to_coco.py

3. Inorder to train the baseline DETR model, run the following command inside detr

!python3 main.py --dataset_file face --data_path ../Datasets/ --output_dir output --resume weights/detr-r50-e632da11.pth

4. Inorder to train the two stage cross attention DETR model, run the following command inside detr

!python3 main.py --dataset_file face --data_path ../Datasets/ --output_dir output

**Note:** DETR.ipynb  is the notebook used to train the models


