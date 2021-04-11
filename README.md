# Face-Mask-Detection
YOLOv3 from darknet has been used to train a custom object detector for Covid Masks

1) Create a folder to save the .txt files that xml_to_yolo.py script outputs (e.g. mask_yolo_data).
2) Execute: python xml_to_yolo.py --input=face_mask_detection\annotations --output=mask_yolo_data
3) Copy the .png images from face_mask_detection\images into mask_yolo_data, so as to have a folder with
   structure like this: 0.png, 0.txt, 1.png, 1.txt, ... n.png, n.txt.
4) Execute: python show_bb.py --input=mask_yolo_data
5) By either closing a window or by pressing 'Enter' a new image is being displayed with its bounding boxes.
   The "Esc" button closes all windows and terminates the program.
