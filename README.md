# SVT-Robotics

Instructions for running and testing the function:

It's simple, just run all the cells. The input parameters required are loadId(str), x(float), y(float).
The output is a dictionary, including the information of robotId, distanceToGoal and batterylevel.

Information about what you'd do next, per above requirements:

I can add a function for error handling, for example, I can check the input type and throw an error if it doesn't match the desired input type.

Besides, to add more flexibility, instead of write the actual url for robots' information in the function, I may include the url as one of the input parameters.

If the problem expands to millions of robots, maybe I'll do a quick scan of the robot's position. For example, firstly select robots with 100 units of horizontal and vertical distance, then calculate the actual distance of these pre-selected robots and select the optimal one. If there is no robot within 100 units of horizontal and vertical distance, then increase the scanning distance, e.g., 200, 400, etc.
