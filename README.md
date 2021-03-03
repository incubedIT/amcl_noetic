# incubed_amcl

Fork from https://github.com/ros-planning/navigation/tree/noetic-devel/amcl at hash 22735aa01f2df383bdb16c26b4882eda8a556bed with some changes.

## Current changes

* Avoid that a negative covariance is stored to the parameter, to avoid not-a-number issues at map-updates
* Possibility to change the scan-topic dynamically
* Added possibility to ignore beams during calculating probability for the given pose
