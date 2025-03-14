# Team Photon Ros2 Weekly Update - 3/11

## 👥 Members
- Harrison Surma
- Zoe Strassner
- Macie Hoff
- Tom Winterton

## 🏆 Accomplishments
- Committed a working convex orange detection ros2 package
- Communicated with Electrical (Nikola) over Hydrophone information
    - Commited to [2025 Hydrophone](https://github.com/MUsurf/Hydrophones-Teensy/tree/2025-hydrophone)

## 🚧 Challenges
- Setting up a custom Ros2 publisher class.<sup>1</sup>
- Docker container from `MUSURF/containerization` wasn't building.<sup>2</sup>

## 🛠 Solutions
- <sup>1</sup> Ros2 custom publishers are not possible purely in python.
- <sup>2</sup> Docker container's package imports from `MUSURF/TapeWorm` were incorrectly identified due to a commit with new folder names.
    - Manually changing the DOCKERFILE in containerization fixed the build. 

## 📚 Resources
- [Python Custom Messages](https://robotics.stackexchange.com/questions/114128/ros2-jazzy-python-custom-messages)<sup>1</sup>

## 🎯 Next Week’s Goals
- Preserve Hydrophone knowledge beyond Tom & Harry.
- Break down Hydrophone tasks.
- Communicate with Alec to fill understanding on Hydrophones.

## 🔍 Additional Notes
- 