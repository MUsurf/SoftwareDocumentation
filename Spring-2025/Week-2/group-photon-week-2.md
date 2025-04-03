# Photon Ros Package Weekly Update - [3/18]

## 👥 Members
- Harry Surma, Macie Hoffman

## 🏆 Accomplishments
- Ensured the ROS package was working with the latest version of the docker container
    - Steps to ensure package works
        - Removed dependencies from package.xml of image_recognition except `cv_bridge` and `python3-opencv`
        - Added to DOCKERFILE
            - added image_recognition package to --mount-type run line
        - Add image_recognition to TapeWorm folder
        - (Optional) Change run.sh to test
- Merged `packageAttempt` into `main` on [image_recognition](https://github.com/MUsurf/image_recognition)
    - Applied changes to get working
- Updated `/Software_Documentation` actions to work as intended

## 🚧 Challenges
- Knowing what dependencies can be listed in package.xml
    - Solution: [Ros Distro Repository list of possible dependencies](https://github.com/ros/rosdistro/blob/master/rosdep/python.yaml)
- Ros Distro repo list lies and says `python-opencv` is an option
    - Solution: Listen to George and use `python3-opencv`

## 📚 Resources
- [RosDep dependencies list](https://github.com/ros/rosdistro/blob/master/rosdep/python.yaml)
