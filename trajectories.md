---
layout: page
title: Trajectories
---

The four outdoor trajectories can be visualized on the interactive map below. Outdoor trajectories. <span style="font-family: monospace;">Urban01</span> in <span style="color: red; font-weight: bold;">red</span>, <span style="font-family: monospace;">Urban02</span> in <span style="color: blue; font-weight: bold;">blue</span>, <span style="font-family: monospace;">Urban03</span> in <span style="color: cyan; font-weight: bold;">cyan</span>, and <span style="font-family: monospace;">Urban04</span> in <span style="color: goldenrod; font-weight: bold;">yellow</span>.

<div style="text-align: center;">
  <iframe src="https://www.google.com/maps/d/u/0/embed?mid=15RbG2iCkygBUAvPHpycijGC5UoVxvPE&ehbc=2E312F&noprof=1" width="100%" height="480"></iframe>
</div>

The indoor trajectories are presented below. Segments are colored according to their height, with the <span style="color: goldenrod; font-weight: bold;">yellow</span> portion recorded outside the garage and the <span style="color: red; font-weight: bold;">red</span> portion recorded inside. The garage ceiling is rendered transparent to enhance visualization.

<div style="text-align: center;">
  <img src="/assets/img/indoor_trajectories.png" alt="Indoor trajectories" width="100%">
</div>

We summarize the metadata of the trajectories in the table below. The outdoor trajectories were repeated at night to provide data for computer vision practitioners interested in exploring the challenges of vehicle navigation using cameras in low-light conditions.

<div style="width: 100%; display: flex; justify-content: center;">
  <table border="1" cellspacing="0" cellpadding="5" style="width: 1280px; margin: 0 auto;">
    <thead>
      <tr>
        <th>Trajectory</th>
        <th>Length (km)</th>
        <th>Duration (min)</th>
        <th>Avg. Speed (km/h)</th>
        <th>Max. Speed (km/h)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="text-align: center;">Urban01</td>
        <td style="text-align: center;">8.70</td>
        <td style="text-align: center;">36.63</td>
        <td style="text-align: center;">14.24</td>
        <td style="text-align: center;">42.15</td>
      </tr>
      <tr>
        <td style="text-align: center;">Urban02</td>
        <td style="text-align: center;">6.78</td>
        <td style="text-align: center;">23.58</td>
        <td style="text-align: center;">17.26</td>
        <td style="text-align: center;">40.49</td>
      </tr>
      <tr>
        <td style="text-align: center;">Urban03</td>
        <td style="text-align: center;">5.21</td>
        <td style="text-align: center;">21.53</td>
        <td style="text-align: center;">12.12</td>
        <td style="text-align: center;">43.05</td>
      </tr>
      <tr>
        <td style="text-align: center;">Urban04</td>
        <td style="text-align: center;">4.87</td>
        <td style="text-align: center;">17.75</td>
        <td style="text-align: center;">16.46</td>
        <td style="text-align: center;">44.57</td>
      </tr>
      <tr>
        <td style="text-align: center;">Indoor01</td>
        <td style="text-align: center;">1.25</td>
        <td style="text-align: center;">7.03</td>
        <td style="text-align: center;">10.63</td>
        <td style="text-align: center;">23.52</td>
      </tr>
      <tr>
        <td style="text-align: center;">Indoor02</td>
        <td style="text-align: center;">0.97</td>
        <td style="text-align: center;">5.86</td>
        <td style="text-align: center;">9.93</td>
        <td style="text-align: center;">22.13</td>
      </tr>
      <tr>
        <td style="text-align: center;">Indoor03</td>
        <td style="text-align: center;">1.27</td>
        <td style="text-align: center;">8.43</td>
        <td style="text-align: center;">9.00</td>
        <td style="text-align: center;">22.20</td>
      </tr>
    </tbody>
  </table>
</div>