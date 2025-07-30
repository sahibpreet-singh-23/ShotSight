# ShotSight
Just imagine you are watching a golf match. 
The ball rolls slowly toward the hole. Your eyes are locked in. 
Will it go in? 
That exciting moment is what we call the perfect shot.

ShotSight is a project that utilizes Computer Vision to detect golf hole and track golf ball, while also telling when a putt is achieved.

The system utilizes YOLO11n model trained for detection of golf_ball and golf_hole. While training the model, parameters provided were as followed:
imgsz = 640*640 (Image Size)
batch = 16 (Batch Size)
lr0 = 0.01 (Learning Rate)
optimzer = SGD (Stochastic Gradient Descent)

The model gives an accuracy of 90.4% on detection of ball and 100% accuracy on detection of hole.
The putt is achieved when the bounding boxes of both ball and hole overlap with a threshold of 0.2.
