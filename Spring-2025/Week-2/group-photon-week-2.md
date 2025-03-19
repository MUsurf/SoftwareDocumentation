# Photon Ros Package Weekly Update - [3/18]

## 👥 Members
- Harry Surma, Macie Hoffman

## 🏆 Accomplishments
- Ensured the ROS package was working with the latest version of the docker container
    - Steps to ensure package works
        - Removed dependencies from package.xml of image_recognition except `cv_bridge`
        - Added to DOCKERFILE
            - pip install python-opencv
            - added image_recognition package to --mount-type run line
        - Add image_recognition to TapeWorm folder
        - (Optional) Change run.sh to test

## 🚧 Challenges
- What issues did we run into?

## 🛠 Solutions
- How were issues resolved?

## 📚 Resources
- Relevant resources like links, repositories, articles, documentation.

## 🎯 Next Week’s Goals
- What is next week, make it a good place to look at to start Tuesday.

## 🔍 Additional Notes
- Any details that don't fit elsewhere.
