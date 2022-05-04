# incubed_amcl

Fork from https://github.com/ros-planning/navigation/tree/noetic-devel/amcl at hash 22735aa01f2df383bdb16c26b4882eda8a556bed with some changes.

## Current changes

* The name of the map topic can be changed via reconfiguration
* Fixed uninitialized frame names becoming valid after the tf_prefix is removed
* Avoid that a negative covariance is stored to the parameter, to avoid not-a-number issues at map-updates
* Possibility to change the scan-topic dynamically
* Added possibility to ignore beams during calculating probability for the given pose
* Avoid that the amcl node writes its last pose to the parameter server