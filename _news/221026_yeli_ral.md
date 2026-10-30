---
layout: post
title:  🎉 New Paper Accepted at IEEE Robotics and Automation Letters (RA-L) by Ye Li
date: 2026-10-22 15:30:00-0400
inline: false
related_posts: false
---

Ye Li, together with Mal Fazliu, Yewei Huang, Alberto Quattrini Li, Brendan Englot, and Cunjia Liu, has published a new paper, [VibeIT: Variable-Resolution Virtual Map Guided Belief-Space Informed Tree Search for ASV Exploration](https://ieeexplore.ieee.org/document/11745973), addressing a key challenge in autonomous surface vehicle (ASV) exploration: planning reliable and efficient exploration paths in nearshore environments where GNSS signals may be obstructed and localisation uncertainty is affected by environmental disturbances such as wind and ocean currents.

The work introduces VibeIT, a novel exploration planning framework that uses a Variable-Resolution Virtual Map (VRVM) to represent mapping uncertainty and guide trajectory generation. Rather than relying on random sampling alone, the proposed approach transforms uncertainty information from the virtual map into a spatial information field that guides tree expansion and candidate trajectory generation towards regions with high information content.

A central contribution of the study is an information-guided tree search strategy that balances the exploration of previously unexplored areas with the revisitation of previously observed regions. By biasing sampling and trajectory expansion towards informative regions and selecting optimal trajectories using a virtual-map-based criterion, VibeIT enables more focused and effective exploration.

The proposed framework is evaluated in the VRX Gazebo simulator against four representative autonomous exploration planners. The results demonstrate that VibeIT achieves higher map coverage and lower localisation error across the tested scenarios, highlighting its potential to improve autonomous exploration in challenging nearshore environments.