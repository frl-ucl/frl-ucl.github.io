---
layout: post
title:  🎉 Papers Accepted for ICRA 2026 Vienna
date: 2026-01-31 18:00:00-0400
inline: false
related_posts: false
---

We are pleased to share that a new paper from the FRL Group has been accepted to **ICRA 2026**, one of the leading international conferences in robotics.

The work addresses a challenging failure scenario in marine robotics: when an unmanned surface vehicle loses most of its thrust, conventional control methods become ineffective due to severe actuation limits.

Rather than treating wind and waves purely as disturbances to reject, the proposed approach exploits environmental forces as **virtual actuators**. An environment-assisted model predictive control (MPC) framework adaptively determines how much to rely on these forces based on fault severity and prediction confidence, combining learning-based force prediction with reachability-aware planning and MPC.

The resulting system achieves over **91% mission success** under **95% thruster degradation**, a regime in which standard control approaches fail completely. This demonstrates the potential of environment-aware control for resilient and fault-tolerant autonomous marine systems.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/icra-yang.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>   
