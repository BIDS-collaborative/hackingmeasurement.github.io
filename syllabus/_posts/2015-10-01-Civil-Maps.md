---
title: Civil Maps
author: Dav Clark
presenters: Fabien Chraim
layout: class
---

## Background information

[Civil Maps](https://civilmaps.com/) enables on-demand perception and actuation
of the world around us, by collecting and analyzing spatial data.

## Tentative plan

 - The evolution of surveying (in history, and in recent times)
 - Lidar and photogrammetry technologies: point clouds, maps and reports
 - The data problem (traditional approaches)
 - Civil Maps approach: AI / Machine Vision solutions
 - CM system architecture
 - CM technical metrics (performance)
 - Vision and future directions

## Notes

**Basic idea** CivilMaps generates 3D instead of 2D for surveying / planning.
They can do more, faster, for cheaper.

History of Surveying goes all the way back to primitive sites like Stonehenge.

### Sensors

- **LIDAR** laser equivalent of RADAR, yields a point cloud
- **Camera** gets RGB value for each point from (close to) the same point of
  view
- Or, you can do multi-spectral LIDAR

### How is this different than, e.g., Google street view?

This is a true 3D model constructed from points in a 3D space. Google street
view is a 2D representation that allows us to get some 3D.

Can clearly identify individual objects in space. Application: figure out how
high your train could be on a given stretch of track.

### What are the limitations of the current system?

The browser can only handle so much data.

### General Challenges

Standard "big data" story - can acquire data much faster than we can process it. Manual labelling of assets is very cumbersome.

How to quantify error? Points allow for a straightforward distance. Given the lack of standard, report a transparently computed measure of difference between manual and automatic labels.

## Demo

- You can upload your own data (for now) [here](https://civilmaps.com/).
- Can choose features from a menu.
- Technology can work with a ~$500 LIDAR (as opposed to ~$100,000 survey quality LIDAR)

### Visualizer Links

- [island](https://node.civilmaps.com/visual/550ca0e69442bfd442ee5ef6.00a708a5-fea1-c5a3-bd6e-faaef34ecead/693917.5405360516,3915976.7794604735,275.0764393265107/0.6173168443824303,0,0.9578275973159768)

- [something else](https://node.civilmaps.com/visual/55fbef3de514d11105fd3403.f5b09c4e-e31d-307a-c80d-da36c211fb7e/-27430.733744400124,-37839.22910376916,43.01418029312265/1.5748710254376872,0,-1.6741516551377538)

- [yet another thing](https://node.civilmaps.com/visual/550ca0e69442bfd442ee5ef6.bf1bb73e-7bdc-9ed6-30b8-d71adfc80df7/481139.2151762079,3769643.8248684574,356.1442605330743/1.3385385041559645,0,4.18742577800959)

- [and another](https://node.civilmaps.com/visual/550ca0e69442bfd442ee5ef6.41393f92-0fa0-6fe7-5bab-626bb76f3dcc/701000.680219981,3912857.3267551633,347.3457447202293/1.3140903122992331,0,-0.19033753536407258)

- [lastly](https://node.civilmaps.com/visual/54ea22f146fef74337aa52cf.bd6a52f2-a59e-9795-9200-2ae7e990de41/333874.1676404711,4901851.262021269,326.29294040128923/0.9962638181617431,0,-1.0458331244197947)

### Barriers to humanitarian or conservation work

- Once spatial discriminations are complex (broken buildings, different
  vegetation), the AI isn't there yet, but this should be possible.
- Identifying obstacles in roads could be a good application.
