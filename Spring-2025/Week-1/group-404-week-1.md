# Team Photon Ros2 Weekly Update - 3/11

## 👥 Members
- Harrison Surma
- Zoe Strassner
- Macie Hoff
- Tom Winterton

## 🏆 Accomplishments
- Committed a working convex orange detection ros2 package

## 🚧 Challenges
- Setting up a custom Ros2 publisher class.
- Docker container from `MUSURF/containerization` wasn't building.

## 🛠 Solutions
- Ros2 custom publishers are not possible purely in python.
- Docker container's package imports from `MUSURF/TapeWorm` were incorrectly identified due to a commit with new folder names.
    - Manually changing the DOCKERFILE in containerization fixed the build. 

## 📚 Resources
- [Python Custom Messages](https://robotics.stackexchange.com/questions/114128/ros2-jazzy-python-custom-messages)

## 🎯 Next Week’s Goals
- Start a ROS2 Package for Hydrophones.
- Better follow Docker best practices.

## 🔍 Additional Notes
- 