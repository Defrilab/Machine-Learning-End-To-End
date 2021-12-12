python train.py --img 416 --batch 3 --epochs 10 --data ./data/coco.yml --weights ./weights/yolov5x6.pt
python detect.py --img 416 --source ./data/test --weights ./weights/yolov5x6.pt --conf-thres 0.4
python detect.py --img 416 --source 0 --weights ./weights/yolov5x6.pt --conf-thres 0.4 // for streaming from camera