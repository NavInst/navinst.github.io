---
layout: page
title: Platform
---

<div style="text-align: center;">
  <img src="/assets/img/coordsys.png" alt="NavINST platform" width="640">
</div>

<div style="text-align: center;">
  <table border="1" cellspacing="0" cellpadding="5">
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
        <td><a href="https://novatel.com/products/gnss-inertial-navigation-systems/imus/kvh1750">KVH1750</a></td>
        <td>IMU</td>
        <td>1</td>
        <td>200</td>
        <td>/novatel/imu</td>
        <td>sensor_msgs/Imu</td>
      </tr>
      <tr>
        <td>b</td>
        <td>Xsens MTi-670G</td>
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
          sensor_msgs/Imu<br/>
          sensor_msgs/NavSatFix<br/>
          geometry_msgs/Vector3Stamped<br/>
          sensor_msgs/FluidPressure<br/>
          sensor_msgs/Temperature<br/>
          geometry_msgs/QuaternionStamped<br/>
          geometry_msgs/Vector3Stamped<br/>
          geometry_msgs/TwistStamped
        </td>
      </tr>
      <tr>
        <td>c</td>
        <td>Velodyne VLP-16</td>
        <td>3D Mechanical LiDAR</td>
        <td>1</td>
        <td>10</td>
        <td>/velodyne/lidar/points</td>
        <td>sensor_msgs/PointCloud2</td>
      </tr>
      <tr>
        <td>d</td>
        <td>Livox HAP</td>
        <td>3D Solid-state LiDAR</td>
        <td>1</td>
        <td>10</td>
        <td>
          /livox/lidar/points<br/>
          /livox/lidar/imu
        </td>
        <td>
          sensor_msgs/PointCloud2<br/>
          sensor_msgs/Imu
        </td>
      </tr>
      <tr>
        <td>e</td>
        <td>Luxonis OAK-1 W PoE</td>
        <td>Monocular Camera</td>
        <td>1</td>
        <td>30</td>
        <td>
          /oak/camera_info<br/>
          /oak/image_raw_color/compressed
        </td>
        <td>
          sensor_msgs/CameraInfo<br/>
          sensor_msgs/CompressedImage
        </td>
      </tr>
      <tr>
        <td>f</td>
        <td>Stereolabs ZED X</td>
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
          sensor_msgs/Imu<br/>
          sensor_msgs/Temperature<br/>
          sensor_msgs/CameraInfo<br/>
          sensor_msgs/CompressedImage<br/>
          sensor_msgs/CameraInfo<br/>
          sensor_msgs/CompressedImage<br/>
          sensor_msgs/Imu<br/>
          sensor_msgs/Temperature<br/>
          sensor_msgs/CameraInfo<br/>
          sensor_msgs/CompressedImage<br/>
          sensor_msgs/CameraInfo<br/>
          sensor_msgs/CompressedImage
        </td>
      </tr>
      <tr>
        <td>g</td>
        <td>Smartmicro UMRR-96 Type 153</td>
        <td>4D Electronic Scan Radar</td>
        <td>4</td>
        <td>20</td>
        <td>
          /smartmicro/radar/front_left<br/>
          /smartmicro/radar/front_right<br/>
          /smartmicro/radar/rear_left<br/>
          /smartmicro/radar/rear_right
        </td>
        <td>sensor_msgs/PointCloud2</td>
      </tr>
      <tr>
        <td>h</td>
        <td>Novatel PwrPak7-E1</td>
        <td>GNSS/IMU</td>
        <td>1</td>
        <td>50</td>
        <td>
          /novatel/imu<br/>
          /novatel/gps
        </td>
        <td>
          sensor_msgs/Imu<br/>
          gps_common/GPSFix
        </td>
      </tr>
      <tr>
        <td>i</td>
        <td>Novatel VEXXIS GNSS-850</td>
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
        <td>OPS241-A</td>
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



