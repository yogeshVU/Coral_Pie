### Coral-Pie: A Geo-Distributed Edge-compute Solution for Space-Time Vehicle Tracking

#### Hardware
Raspberry Pi (Raspbian-lite) + EdgeTPU

#### Dependency
- opencv_depdency/ contains the pre-compiled opencv library for Raspberry Pi
- other_dependency.sh
- edgetpu python library

#### System components
- Camera topology server: archive/cameraTop/camera_topology_server.py contains the camera topology code, config/cameras.json contains the camera location configuration.
- Janusgraph (trajectory storage backend): `docker run -it -p 8182:8182 janusgraph/janusgraph`
- VideoStorage: video_storage/run_video_storage_server.py
- Main camera processing: version1/run.py, version2/rpi1_run.py, version2/rpi2_run.py


