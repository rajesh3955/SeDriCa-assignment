SeDriCa Assignment: Perception Starter Data

Project Overview

This repository contains the SeDriCa perception starter data.All examples are original synthetic.They are teaching cases,not evidence of real-car performance.
Directory Structure & Dataset Details

1. City Environment (Camera & V2X Data)
•	Lane Detection:
o	city/lane: Contains three 24-frame RGB sequences, 480 x 320. 
o	city/calibration.json: Contains four planar point correspondences. 
o	city/lane_reference.csv: Contains true lane centers for evaluation only. 

•	Crossing Detection:
o	city/crossing: Contains three 24-frame RGB sequences. 
o	city/crossing_evidence.csv: Contains noisy scores, speed, distance and V2X messages. 
o	city/crossing_reference.csv: Contains true crossing states for evaluation only. 

2. Race Environment (LiDAR Data)
•	race/scans.csv: Contains five 18-frame LiDAR sequences; an empty cell is a missing return. 
•	race/sensor.json: Contains scan angles, vehicle geometry, corridor bounds and units. 
•	race/scene_reference.csv: Contains obstacle positions for evaluation only. 

3. Localization Route (Odometry Data)
•	localization/reference_scans.csv: Contains eight candidate-place fingerprints. 
•	localization/observed_scans.csv: Contains a 12-step route with noisy odometry. 
•	localization/route_graph.csv: Contains stay/move transitions. 
•	localization/route_reference.csv: Contains true places for evaluation only.
 
Evaluation Guidelines
CRITICAL RULE: Do not use reference labels within prediction functions. 
Author: Rajesh Podilapu | IIT Bombay


