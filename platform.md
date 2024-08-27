---
layout: page
title: Platform
---

<div style="text-align: center; width: 100%">
  <img src="/assets/img/coordsys.png" alt="NavINST platform" width="100%">
</div>

All sensors available on our platform are listed below. For your convenience, we have included links to the manufacturers' websites and corresponding ROS messages. For more technical details, please refer to our paper.

<div style="width: 100%; overflow-x: auto;">
  <table border="1" cellspacing="0" cellpadding="5" style="width: 1460px; margin: 0 auto;">
    <thead>
      <tr>
        <th>Label</th>
        <th>Sensor</th>
        <th>Type</th>
        <th>Qty</th>
        <th>Hz</th>
        <th>Topic Name</th>
        <th>Message Type</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>a</td>
        <td><a href="https://novatel.com/products/gnss-inertial-navigation-systems/imus/kvh1750" target="_blank">KVH1750</a></td>
        <td>IMU</td>
        <td>1</td>
        <td>200</td>
        <td>/novatel/imu</td>
        <td><a href="https://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Imu.html" target="_blank">sensor_msgs/Imu</a></td>
      </tr>
      <tr>
        <td>b</td>
        <td><a href="https://www.movella.com/products/sensor-modules/xsens-mti-670g-gnss-ins" target="_blank">Xsens MTi-670G</a></td>
        <td>GNSS/IMU</td>
        <td>1</td>
        <td>100</td>
        <td>
          /xsens/imu<br/>
          /xsens/gnss<br/>
          /xsens/mag<br/>
          /xsens/pressure<br/>
          /xsens/temperature<br/>
          /xsens/filter/quaternion<br/>
          /xsens/filter/positionlla<br/>
          /xsens/filter/twist
        </td>
        <td>
          <a href="https://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Imu.html" target="_blank">sensor_msgs/Imu</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/NavSatFix.html" target="_blank">sensor_msgs/NavSatFix</a><br/>
          <a href="https://docs.ros.org/en/noetic/api/geometry_msgs/html/msg/Vector3Stamped.html" target="_blank">geometry_msgs/Vector3Stamped</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/FluidPressure.html" target="_blank">sensor_msgs/FluidPressure</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Temperature.html" target="_blank">sensor_msgs/Temperature</a><br/>
          <a href="https://docs.ros.org/en/noetic/api/geometry_msgs/html/msg/QuaternionStamped.html" target="_blank">geometry_msgs/QuaternionStamped</a><br/>
          <a href="https://docs.ros.org/en/noetic/api/geometry_msgs/html/msg/Vector3Stamped.html" target="_blank">geometry_msgs/Vector3Stamped</a><br/>
          <a href="https://docs.ros.org/en/noetic/api/geometry_msgs/html/msg/TwistStamped.html" target="_blank">geometry_msgs/TwistStamped</a>
        </td>
      </tr>
      <tr>
        <td>c</td>
        <td><a href="https://store.clearpathrobotics.com/products/puck" target="_blank">Velodyne VLP-16</a></td>
        <td>3D Mechanical LiDAR</td>
        <td>1</td>
        <td>10</td>
        <td>/velodyne/lidar/points</td>
        <td><a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/PointCloud2.html" target="_blank">sensor_msgs/PointCloud2</a></td>
      </tr>
      <tr>
        <td>d</td>
        <td><a href="https://www.livoxtech.com/hap" target="_blank">Livox HAP</a></td>
        <td>3D Solid-state LiDAR</td>
        <td>1</td>
        <td>10</td>
        <td>
          /livox/lidar/points<br/>
          /livox/lidar/imu
        </td>
        <td>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/PointCloud2.html" target="_blank">sensor_msgs/PointCloud2</a><br/>
          <a href="https://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Imu.html" target="_blank">sensor_msgs/Imu</a>
        </td>
      </tr>
      <tr>
        <td>e</td>
        <td><a href="https://shop.luxonis.com/products/oak-1-w-poe?variant=43854167081183" target="_blank">Luxonis OAK-1 W PoE</a></td>
        <td>Monocular Camera</td>
        <td>1</td>
        <td>30</td>
        <td>
          /oak/camera_info<br/>
          /oak/image_raw_color/compressed
        </td>
        <td>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CameraInfo.html" target="_blank">sensor_msgs/CameraInfo</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CompressedImage.html" target="_blank">sensor_msgs/CompressedImage</a>
        </td>
      </tr>
      <tr>
        <td>f</td>
        <td><a href="https://www.stereolabs.com/en-ca/products/zed-x" target="_blank">Stereolabs ZED X</a></td>
        <td>Stereo Camera</td>
        <td>2</td>
        <td>15</td>
        <td>
          /zedx_left/imu<br/>
          /zedx_left/temperature<br/>
          /zedx_left/camera_left/camera_info<br/>
          /zedx_left/camera_left/image_raw_color/compressed<br/>
          /zedx_left/camera_right/camera_info<br/>
          /zedx_left/camera_right/image_raw_color/compressed<br/>
          /zedx_right/imu<br/>
          /zedx_right/temperature<br/>
          /zedx_right/camera_left/camera_info<br/>
          /zedx_right/camera_left/image_raw_color/compressed<br/>
          /zedx_right/camera_right/camera_info<br/>
          /zedx_right/camera_right/image_raw_color/compressed
        </td>
        <td>
          <a href="https://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Imu.html" target="_blank">sensor_msgs/Imu</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Temperature.html" target="_blank">sensor_msgs/Temperature</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CameraInfo.html" target="_blank">sensor_msgs/CameraInfo</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CompressedImage.html" target="_blank">sensor_msgs/CompressedImage</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CameraInfo.html" target="_blank">sensor_msgs/CameraInfo</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CompressedImage.html" target="_blank">sensor_msgs/CompressedImage</a><br/>
          <a href="https://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Imu.html" target="_blank">sensor_msgs/Imu</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Temperature.html" target="_blank">sensor_msgs/Temperature</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CameraInfo.html" target="_blank">sensor_msgs/CameraInfo</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CompressedImage.html" target="_blank">sensor_msgs/CompressedImage</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CameraInfo.html" target="_blank">sensor_msgs/CameraInfo</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/CompressedImage.html" target="_blank">sensor_msgs/CompressedImage</a>
        </td>
      </tr>
      <tr>
        <td>g</td>
        <td><a href="https://autonomoustuff.com/products/smartmicro-automotive-radar-umrr-96" target="_blank">Smartmicro UMRR-96 Type 153</a></td>
        <td>4D Electronic Scan Radar</td>
        <td>4</td>
        <td>20</td>
        <td>
          /smartmicro/radar/front_left<br/>
          /smartmicro/radar/front_right<br/>
          /smartmicro/radar/rear_left<br/>
          /smartmicro/radar/rear_right
        </td>
        <td><a href="http://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/PointCloud2.html" target="_blank">sensor_msgs/PointCloud2</a></td>
      </tr>
      <tr>
        <td>h</td>
        <td><a href="https://novatel.com/products/gnss-inertial-navigation-systems/combined-systems/pwrpak7-e1" target="_blank">Novatel PwrPak7-E1</a></td>
        <td>GNSS/IMU</td>
        <td>1</td>
        <td>50</td>
        <td>
          /novatel/imu<br/>
          /novatel/gps
        </td>
        <td>
          <a href="https://docs.ros.org/en/noetic/api/sensor_msgs/html/msg/Imu.html" target="_blank">sensor_msgs/Imu</a><br/>
          <a href="http://docs.ros.org/en/noetic/api/gps_common/html/msg/GPSFix.html" target="_blank">gps_common/GPSFix</a>
        </td>
      </tr>
      <tr>
        <td>i</td>
        <td><a href="https://novatel.com/products/gps-gnss-antennas/vexxis-series-antennas/vexxis-gnss-800-series-antennas" target="_blank">Novatel VEXXIS GNSS-850</a></td>
        <td>GNSS Antenna</td>
        <td>1</td>
        <td>-</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>-</td>
        <td>Automotive Scanner OBDII</td>
        <td>Odometer</td>
        <td>1</td>
        <td>16</td>
        <td>
          /obd2/speed<br/>
          /obd2/rpm<br/>
          /obd2/maf
        </td>
        <td>❑</td>
      </tr>
      <tr>
        <td>-</td>
        <td><a href="https://omnipresense.com/product/ops241-a-short-range-radar-sensor/" target="_blank">OPS241-A</a></td>
        <td>1D Doppler Radar</td>
        <td>1</td>
        <td>18</td>
        <td>/omnipresense/radar/front_bumper</td>
        <td>❑</td>
      </tr>
    </tbody>
  </table>
  <p>❑ custom message.</p>
</div>

We provide a <a href="https://foxglove.dev/" target="_blank">Foxglove Studio</a> <a href="https://github.com/NavInst/dataset/tree/main/visualization" target="_blank">template</a> to facilitate data visualization and monitoring, as shown below. The transformation tree (TF) is also included, allowing users to easily navigate between sensors. In our setup, the KVH1750 (item 'a' in the figure above) serves as the origin.

<div class="row">
    <div class="video-container">
        <video width="100%" autoplay loop muted>
            <source src="/assets/video/setup_demo_foxglove.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

**Importante notes:**
- The linear accelerations of the IMU inside the Livox HAP LiDAR are scaled by G. Therefore, one should reverse the scaling by multiplying the measurements by 9.8.
- The reference system of the indoor trajectories was recorded with the EPSON EP320G IMU installed inside the PwrPak7-E1 instead of the KVH1750 IMU.