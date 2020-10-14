This project is on the multiple objects detection in images with YOLO v3 model. Here a pre-trained YOLO v3 model (trained with huge COCO dataset) has been used to detect various object in images. It not only detects objects in a image but also it creates a bounding box around a particular object and also writes the name of the class that object belongs to (cat/dog/horse/person etc.). It also writes the score (probability) with which that object was detected. YOLO v3 model is based on deep learning model (CNN).
Here, we downloaded 3 different images (dog-bicycle-person.jpg, person-car-horse.jpg, persons-car-dog.jpg) from https://unsplash.com/ for objects detection with YOLO v3. 
Original images can be found in \images\test and result images (after object detection) can be found in \images\res.

Results are quite satisfactory. It could detect all the relevant objects in the images successfully. 

Following parameters are used for YOLO v3 model.

obj_threshold (threshold for object) = 0.4
nms_threshold (threshold for box) = 0.5


Details of Output:

image = person-car-horse.jpg
------------------------------------------------------------
time: 27.94s
class: person, score: 0.49
box coordinate x,y,w,h: [166.26152396 100.88926944  68.1207329  165.10906559]
class: horse, score: 1.00
box coordinate x,y,w,h: [ 54.58498001 142.51217365 242.32938886 194.35351539]
class: car, score: 0.99
box coordinate x,y,w,h: [256.50203228 192.47191107 220.4093188   75.60168716]


image = persons-car-dog.jpg
------------------------------------------------------------
time: 20.56s
class: person, score: 1.00
box coordinate x,y,w,h: [262.1165514   48.7228632  103.76606882 301.12583637]
class: person, score: 0.46
box coordinate x,y,w,h: [382.15705752 178.36940289  14.55458533  36.05409265]
class: dog, score: 0.96
box coordinate x,y,w,h: [370.21049857 259.01699066  96.16820514  90.61459899]
class: car, score: 0.98
box coordinate x,y,w,h: [367.47401953 170.73101997 131.86906278  99.4012773 ]

image = dog-bicycle-person.jpg
------------------------------------------------------------
time: 21.45s
class: person, score: 1.00
box coordinate x,y,w,h: [192.97274947  64.35571611 204.62395251 293.34233701]
class: bicycle, score: 1.00
box coordinate x,y,w,h: [ 38.43025863 112.99792305 349.55060482 295.75549811]
class: dog, score: 1.00
box coordinate x,y,w,h: [167.03544557 403.68953347 266.01412892 196.58558071]
