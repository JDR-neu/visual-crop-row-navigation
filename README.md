# Visual-Servoing based Navigation for Monitoring Row-Crop Fields
---
<div align="center">
	<img src="/img/agribot_vsPoster.png" alt="visualservoing" width="700" title="visualservoing"/>
</div>

In this paper, we propose a framework tailored for
navigation in row-crop fields by exploiting the regular crop-row structure present
in the fields. Our approach uses only the images from on-board cameras without
the need for performing explicit localization or maintaining a map of the field.
It allows the robot to follow the crop-rows accurately and handles the switch to
the next row seamlessly within the same framework. We implemented our approach
using C++ and ROS and thoroughly tested it in several simulated environments with different
shapes and sizes of field

<div align="center">
	<img src="/img/vs_graph.png" alt="visualservoing" width="400" title="visualservoing"/>
</div>

<div align="center">
	<img src="/img/vs_em.png" alt="visualservoing" width="400" title="visualservoing"/>
</div>

<div align="center">
	<img src="/img/motivation.png" alt="visualservoing" width="400" title="visualservoing"/>
</div>

<div align="center">
	<img src="/img/motivation_old.png" alt="visualservoing" width="400" title="visualservoing"/>
</div>


Node: [/agribot_vs]

Publications: 
 * /cmd_vel [geometry_msgs/Twist]
 * /vs_image [image]
 * /vs_msg [agribot_visualservoing/vs_msg]

Subscriptions: 
 * /amcl_pose [pose]
 * /odom [geometry_msg/odometry]
 * /front/rgb/image_raw [image]
 * /back/rgb/image_raw [image]
 * /zed/camera/left/image_raw [sensor_msgs/Image]

Services: 
 * None

--- 

**Parameters**
 * None
---
- add description
- add pics
- add videos

## License

This project is licensed under the FreeBSD License. See the LICENSE.txt file for details.
