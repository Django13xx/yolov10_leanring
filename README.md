# Thanks to AI百晓生!!!
This project is based on the tutorial below:
<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=1605877535&bvid=BV1jm421579G&cid=1593642215&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

# yolov10_leanring
The example usage of YOLO base model. (Default setting and ready for trainning)

# For start

1. Active the virtual environment
```
venv/Scripts/activate.ps1
```
2. Run the demo file
```
python yolov10-demo.py
```
3. Future optional steps: use my data for training (roboflow)

# Details:
## yolo10 Local deployment

1、install python3.10 and Git 

2、Create the yolov10 folder

3、terminal run the following for installation 
```
pip install supervision labelme  labelme2yolo huggingface_hub google_cloud_audit_log 

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118 pip install git+https://github.com/THU-MIG/yolov10.git
```
## yolo10 camera detection 

1. test the model
```
python yolov10-demo.py
```

2. run the screenshot program
```
python gen-imgs.py
```

3. roboflow online mark

4. use the dataset for training
```
yolo detect train data=yolo10-test/data.yaml model=yolov10n.pt epochs=30 batch=8 imgsz=640 device=0 5、python yolov10-detect.py
```

5. Test the model

## Local annotation tools

1、labelme run the annotation tools

2、labelme2yolo --json_dir D:\github\yolo10\output_images


