Self-driving vehicles are the one's where human drivers are never required to take
control to safely operate the vehicle. Also known as autonomous or “driverless” cars,
they combine sensors and software to control, navigate, and drive the vehicle. 
The project presents a mobile robot which is designed to autonomously navigate through a track by
detecting lanes and centering itself between them by using a camera. We are proposing a
basic and simplest algorithm for tracking and detecting lanes considering cameras'
parameters. This project uses Machine Learning (Convolutional Neural Networks) and
OpenCV library for digital image processing under LINUX environment.

In this project, we were able to successfully predict the steering angles using
convolutional neural networks and were able to understand the inner details of
convolutional neural networks along with the way they can be tuned. We also
demonstrated that CNN’s are able to learn the entire task of lane and road following
without manual decomposition into road or lane marking detection, semantic abstraction,
path planning, and control. A small amount of training data from less than a hundred
hours of driving was sufficient to train the car to operate in diverse conditions, on
highways, local and residential roads in sunny, cloudy, and rainy conditions. An
interesting caveat to this is that the system was able to successfully drive on the roads that
it had been trained on. Autonomous systems for vehicles that don’t use the Udacity
simulator require a greater robustness as they have to take into consideration roads that
haven’t been driven on and a greater amount of obstacles such as pedestrians and stop
signs.The CNN is able to learn meaningful road features from a very sparse training
signal (steering alone). The system learns for example to detect the outline of a road
without the need of explicit labels during training.

Future Scope
We have several ideas to improve the performance of the self driving car.The first idea
would be to add the feature of speed to the CNN so that when the simulator in
autonomous mode, it is using the predicted speed making the movement appear to be
more realistic. The need for this element to be added came from observing the simulator
driving in autonomous mode after training the car and noticing that after it accelerates to
the maximum speed, the car will automatically slow down to the minimum speed making
it appear unrealistic.
Another possible improvement would be to consider each of the cameras separately and
create CNN models using each stream of images to create a distinct steering command
coming from the left, center, and right model. Then averaging the three of these to get
amore accurate prediction. We would expect that the majority of the time, this model
would have accurate predictions but if one model predicts a steering angle that is very
unlike the other two, then it would skew the steering angle in an unexpected direction.
As self driving vehicle is the Future as the resources are depriving on daily basis so the
alternative. Talking about the scope is insignificant talk as they are future so one should
be concentrating on how to improvise the performance and how it should be shaped in
order to give effective performance for the consumers.
On the other part if we talk about solely on self driving electric vehicle,it will be seen on
roads in coming years eliminating present vehicles with better performance and cost
effectiveness. Thus we can say that self driving electric cars will dominate the vehicle
market and the extent to which it will improvise will be observed in few decades.
The pipeline is able to predict safe driving behavior for the self-driving car in both the
tracks of Udacity Simulator. The proposed work can be extended to real scenarios as
well. This can be done by collecting good driving behavior on real roads and then using
that data and feeding it in the model for the predictions. The dataset used for training can
be Waymo Open Dataset or Udacity’s Open Source dataset. The model can further be
made more complex or tweaked to increase accuracy on real road scenarios as well. Also,
this model can be trained for real road images from several cameras on the hood of the
car i.e. center, left and right camera images can be used as input. Hence, the model once
trained can be deployed in a real self-driving car as well.
