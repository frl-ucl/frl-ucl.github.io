---
layout: page
title: Research
permalink: /projects/
description:  "Our group is dedicated to advancing autonomous systems through cutting-edge research in three core areas: Reliable Sensing and Perception, Intelligent Planning and Decision Making, and Advanced Robust Control. Our mission is to develop resilient technologies that enhance system reliability by integrating sophisticated sensing, perception, and adaptive control frameworks. By leveraging the latest advances in machine learning, optimization, and control theory, we address real-world challenges, enabling autonomous platforms to navigate and operate effectively in complex, dynamic environments."
nav: true
nav_order: 3
display_categories: [Reliable Sensing and Perception, Intelligent Planning and Decision Making, Advanced Robust Control]
horizontal: false
---

<h2 class="category">Reliable Sensing and Perception</h2>
<div style="width: 100%; height: 0.5px; background-color: rgba(0, 0, 0, 0.15); margin-top: -8px; margin-bottom: 20px;"></div>

<p style="text-align: justify;">We develop deep learning algorithms for robust object detection in challenging marine environments, enabling reliable perception under varying sea states, lighting conditions, and complex port settings. Our work focuses on enhancing the accuracy of underwater and surface object detection, ensuring the safe and efficient operation of autonomous maritime systems.</p>

 <!-- -----------------------------------------------VISUAL DETECTION-->
<p style="font-size: 25px;"><b>Multi-sensor-based</b></p>

<p style="text-align: justify;">In collaboration with Port of London Authority, our research group conducted a series of data collection trials on the River Thames. We used multiple perception sensors including 3D LiDAR, high-resolution cameras, sound velocity profilers, etc. onboard a survey vessel to achieve a comprehensive autonomous understanding of traffic in busy waterways. We are grateful for the support from Port of London Authority and our funder, EPSRC.</p>

<div class="row justify-content-center align-items-center" style="margin-top: 1.5rem;">
    <div class="col-md-6 mb-3 mb-md-0">
        {% include video.liquid path="assets/img/projects/lidar-based.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-md-6">
        {% include figure.liquid loading="eager" path="assets/img/projects/marina-still.gif" title="Marina Still" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<!-- References -->
Research Output: [[Ocean Engineering '15](https://www.sciencedirect.com/science/article/pii/S0029801815000165?casa_token=IMX39rYW6V4AAAAA:w9y5P73ZHORoiSLiH5b4xtypu4Pq6CDq_vpJrVoF6jkCS80hfiVzDHFh1dBOtdBYIGBqKul5Qg)] [[T-ASE '24](https://ieeexplore.ieee.org/abstract/document/10443430/?casa_token=c6TqEj3UEyoAAAAA:-HAYweS-tQeqPO0Xdvq0eYUehgL5UwZJzLM5NVSIsA-oDyaRHYZuHUvUm1DyX-VSWzd3m9Pw)], [[Ocean Engineering '24](https://www.sciencedirect.com/science/article/pii/S002980182402626X)]

<br>

 <!-- ----------------------------------------------- LIDAR -->
<p style="font-size: 25px;"><b>Radar-based</b></p>
We recently conducted data collection trials aboard a Port of London Authority (PLA) survey boat at Gravesend. These trials are a crucial step in enhancing autonomous vessel perception and navigation. Autonomous marine navigation has made significant strides, but harsh weather conditions still pose a major challenge. To bridge this gap, we are exploring the potential of 360° high-definition imaging radar to enable all-weather autonomous navigation for marine vessels.

<div class="row justify-content-center align-items-center" style="margin-top: 1.5rem;">
    <div class="col-md-6 mb-3 mb-md-0">
        {% include figure.liquid path="assets/video/gravesendtesting.gif" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-md-6">
        {% include figure.liquid path="assets/video/gravesenddata.gif" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

<!-- References -->
<!-- Research Output: [[Ocean Engineering '15](https://www.sciencedirect.com/science/article/pii/S0029801815000165?casa_token=IMX39rYW6V4AAAAA:w9y5P73ZHORoiSLiH5b4xtypu4Pq6CDq_vpJrVoF6jkCS80hfiVzDHFh1dBOtdBYIGBqKul5Qg)] -->

<br>

<p style="font-size: 25px;"><b>Uncertainty-aware LiDAR-based Vessel Detection</b></p>

<p style="text-align: justify;">
This work introduces MPCD and U-MPCD, LiDAR-based point cloud detectors designed for autonomous surface vessels operating in complex and high-traffic waterways. By combining fine-grained local geometric features with global multiscale representations, MPCD achieves a <b>12.8%</b> improvement over the benchmark.
</p>

<p style="text-align: justify;">
U-MPCD extends this framework with explicit modeling of both <i>epistemic</i> and <i>aleatoric</i> uncertainty, improving detection performance by a further <b>2%</b> while maintaining <b>15 Hz</b> real-time inference. The resulting system provides not only accurate detections but also calibrated confidence estimates that are critical for safe autonomous navigation.
</p>

<p style="text-align: justify;">
To support evaluation in realistic conditions, a large-scale LiDAR dataset was collected in the busy central section of the River Thames, covering four days of operations (six hours per day) and approximately <b>11.4 km</b> of dense maritime traffic. The dataset captures one of the most challenging urban waterway environments for vessel detection and is fully open-sourced to support the wider research community.
</p>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/xie-2025.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>   
<!-- References -->
Research Output: [[IEEE Journal of Oceanic Engineering '25](https://ieeexplore.ieee.org/abstract/document/11244833/)] 


<br>

<p style="font-size: 25px;"><b>Graph-based AIS Trajectory Intelligence</b></p>

<p style="text-align: justify;">
This work introduces a graph-based framework for modelling AIS vessel trajectories. Rather than representing AIS messages as time series or images, each trajectory segment is modelled as a directed acyclic graph, enabling the explicit capture of spatial, temporal, and geometric dependencies in vessel motion.
</p>

<p style="text-align: justify;">
A hierarchical graph neural network with feature-level attention is proposed to refine both node and edge representations within these linear trajectory graphs. This attention mechanism allows the model to focus on the most informative attributes at each level, a capability that is rarely explored in maritime analytics.
</p>

<p style="text-align: justify;">
The resulting system achieves <b>98% classification accuracy</b> and <b>99% AUC–ROC</b> on large-scale AIS data collected from UK waters, demonstrating strong performance for vessel behaviour analysis. The framework has significant potential for applications including emissions modelling, maritime monitoring, risk and compliance, and autonomous navigation.
</p>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/nana-2026.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>   
<!-- References -->
Research Output: [[Advanced Engineering Informatics '26](https://www.sciencedirect.com/science/article/pii/S1474034625009759?via%3Dihub)] 

<b>




<!-- =================================================================================================== -->








<h2 class="category">Intelligent Planning and Decision Making</h2>
<div style="width: 100%; height: 0.5px; background-color: rgba(0, 0, 0, 0.15); margin-top: -8px; margin-bottom: 20px;"></div>

<p style="text-align: justify;">We design intelligent planning algorithms that enable autonomous systems to make adaptive decisions in dynamic and unpredictable environments. By leveraging deep learning and optimization techniques, our work focuses on enhancing the ability of robots to navigate complex scenarios, efficiently allocate resources, and respond to changing conditions in real time. This ensures robust and reliable performance in challenging operational settings, from marine environments to urban spaces.</p>


<!-- -----------------------------------------------PATH PLANNING -->
<p style="font-size: 25px;"><b>Path and Trajectory Planning</b></p>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/usv-planning.gif" title="USV Planning" class="img-fluid rounded z-depth-1 half-width" %}
    </div>
</div>
<!-- References -->
Research Output: [[IEEE Transactions on Instrumentation and Measurement '21](https://ieeexplore.ieee.org/abstract/document/9464268/?casa_token=xJJkKh9AYkUAAAAA:s68yg7hLqvpGsqWB2nQ8p6F9jQb0u4mnO1H5oZqlk7Kwj5MIZQvGuLkEtX9kg06F4dv4fnvC)], [[Applied Ocean Research '19](https://www.sciencedirect.com/science/article/pii/S0141118718302621?casa_token=pndx6v_EFHsAAAAA:BYu_Cyjyi3AEaCTGcbggLppgLWJOoIPOz5vVXi39JL6O5HXxa1D74WDz2wxx_q-ODZ7QX_nEbA)], [[Sensors '19](https://www.mdpi.com/1424-8220/19/18/4055)], [[Ocean Engineering '17](https://www.sciencedirect.com/science/article/pii/S0029801816305182?casa_token=OVW8bTHOon0AAAAA:nTcfXXGVtgPDIF3KuQUXm7A2paErhWpZ-3kMMDH9GX984LhggZSIG5KjVMbhM69lqgyoASg0ew)]

 <!-- ----------------------------------------------- TASK PLANNING -->
<br>
<p style="font-size: 25px;"><b>Task allocation for multi-robot systems</b></p>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/task-planning.png" title="Task Planning" class="img-fluid rounded z-depth-1 half-width" %}
    </div>
</div>   
<!-- References -->
Research Output: [[Ocean Engineering '22](https://www.sciencedirect.com/science/article/pii/S002980182200720X?casa_token=0NAkQ-w0MOsAAAAA:Amga1-4TH0LBdu3o0Yyk4De0pNf7Zt4AXn5yBKmpnRrCURIrxXuJS0FWsnVvXHlum_f9D1X7XQ)], [[IEEE Journal of Oceanic Engineering '22](https://ieeexplore.ieee.org/abstract/document/9864318/?casa_token=rlxA7EZ9DzYAAAAA:a5IJJu9FKzgGasAa3WiIwIXrkrziGv9RsMhihLeGc-kXN60XqHGAU1xADil9fEIyCN0P1cI2)], [[IROS '21](https://ieeexplore.ieee.org/abstract/document/9636614?casa_token=gmuRwbUBmMYAAAAA:MD-dptuROFDv-_fPcY8_LmaaOW7BgW3djtOEEtXMn5uFuTGIL_DTOCnutKl7ZW95fb9-qaie)]

 <!-- ----------------------------------------------- AUTONOMOUS EXPLORATION AND MAPPING -->
<br>
<p style="font-size: 25px;"><b>Autonomous exploration and mapping</b></p>
We have developed an active SLAM framework built around a virtual map to enable USVs to carry out autonomous exploration and mapping.  In feature-sparse marine environments, our approach explicitly models pose uncertainty and sensor error to predict the positional uncertainty of latent landmarks within a given region.  By steering exploration toward areas where virtual map uncertainty is reduced, USVs can maintain robust localization and reliably detect loop closures throughout their missions.
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/virtualmap.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>   
<!-- References
Research Output: [[Ocean Engineering '22](https://www.sciencedirect.com/science/article/pii/S002980182200720X?casa_token=0NAkQ-w0MOsAAAAA:Amga1-4TH0LBdu3o0Yyk4De0pNf7Zt4AXn5yBKmpnRrCURIrxXuJS0FWsnVvXHlum_f9D1X7XQ)], [[IEEE Journal of Oceanic Engineering '22](https://ieeexplore.ieee.org/abstract/document/9864318/?casa_token=rlxA7EZ9DzYAAAAA:a5IJJu9FKzgGasAa3WiIwIXrkrziGv9RsMhihLeGc-kXN60XqHGAU1xADil9fEIyCN0P1cI2)], [[IROS '21](https://ieeexplore.ieee.org/abstract/document/9636614?casa_token=gmuRwbUBmMYAAAAA:MD-dptuROFDv-_fPcY8_LmaaOW7BgW3djtOEEtXMn5uFuTGIL_DTOCnutKl7ZW95fb9-qaie)] -->


<br>






<!-- =================================================================================================== -->

<h2 class="category">Advanced Robust Control</h2>
<div style="width: 100%; height: 0.5px; background-color: rgba(0, 0, 0, 0.15); margin-top: -8px; margin-bottom: 20px;"></div>

<p style="text-align: justify;">We develop advanced control strategies that ensure robust and stable operation of autonomous systems in challenging real-world conditions. By integrating modern control theory, adaptive algorithms, and machine learning techniques, our work focuses on designing controllers that can handle uncertainties, disturbances, and model variations. This enables autonomous platforms to maintain reliable performance and safety across diverse operational scenarios, from marine environments to dynamic urban settings.</p>

<p style="font-size: 25px;"><b>Environment-assisted Fault-Tolerant Control</b></p>

<p style="text-align: justify;">
This work addresses a critical failure scenario in marine robotics: when an unmanned surface vehicle loses most of its thrust, conventional controllers become ineffective due to severe actuation limits.
</p>

<p style="text-align: justify;">
Rather than treating wind and waves purely as disturbances to be rejected, the proposed approach exploits environmental forces as <i>virtual actuators</i>. An environment-assisted model predictive control framework adaptively determines how much to rely on these forces based on fault severity and prediction confidence, integrating learning-based force prediction with reachability-aware planning and MPC.
</p>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/icra-yang.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>   

<br>
