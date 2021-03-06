# Self Driving Car Lane Detection Project

in this project our goal is to write software pipeline that identify the lane boundaries in a
video from a front-facing camera on a car.

## This Project is done by:
- Zyad Hassan Hosney 1806090
- Dina Ibrahim Elkady 18Q3800


## Steps of this project are the following:

### Phase 1

- Use  RGB, LAB, HSL color transforms, sobel gradients with each agnitude and direction and canny edge detection to create a thresholded binary image.
- Apply a perspective transform to the resulted binary image ("birds-eye view").
- Using sliding window algorithm to detect lane pixels and fit to find the lane boundary.
- Determine the curvature of the lane and vehicle position with respect to center.
- Warp the detected lane boundaries back onto the original image.
- Output image/video with lane well detected



https://user-images.githubusercontent.com/85132939/170764581-790ca035-b528-4eca-92bb-98674f935976.mp4


### Phase 2

- Apply yolo v3 algorithm


![image](https://user-images.githubusercontent.com/85132939/170764401-075921f1-d2bf-48b2-bd1f-42cbe3eccda1.png)

### Steps have been described correctly in the project notebooks `Self_Driving_Car_Lane_Lines_Detection.ipynb` and `Phase 2 Pipeline.ipynb`

> Note: for running Project Phase 1 in Anaconda Prompt you must download both `self_car.ipynb` and `test_car.py` files in the same directory, specify the directory in your cmd and then call `python test_car.py path_in path_out --type 0 --debug 1 --subclip True --subtime 3` for example if you want to show debugging mode and subclib is for gettin short video to reduce the processing time and its default value is 'False' with zero subtime and the type attribute 0 for video and 1 for image.

> Note: for running Project Phase 2 in Anaconda Prompt you must download both `Phase_2_Pipeline2.ipynb` and `test_car_phase2.py` files in the same directory, specify the directory in your cmd and then call `python test_car_phase2.py path_in path_out --type 0` for example, the type attribute 0 for video and 1 for image.
