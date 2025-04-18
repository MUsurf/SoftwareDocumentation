# State Machine: State Machine Weekly Update - [4/15]

## 👥 Members
- Charles Bacher
- Raquel Fellman
- Max Welch
- Elijah VanDyne
- Kaden Culbertson
- Harry SomethingWithAnS
- Jack

## 🏆 Accomplishments
- Defined states for Collecting Data Task
- Defined states for Navigate the Channel Task
- Reviewed Handbook
- Enumerating State Machine Workings
    - Have supervisor on top of highest level state machine
    - Supervisor double checks the output actions don't violate planes

## 🚧 Challenges
- Lack of clarity on task responsibilities
- Deciding Scope of State Machine
- Deciding between states taking purely finite steps or continuous actions
    - Purely Finite: A finished state just represents the next step is chosen and states heavily iterate
    - Continuous: A finished state represents a finished task. Error handling is far more self-reliant
        - Don't let the sub try and pass the 4 planes.
        - If sub tries to leave the 4 planes remove the vector movement towards the disallowed plane and allow remaining vector
- Use camera to try and derive if near a wall or not, slow if not sure near a wall
    - Heuristic for wall? (If center vertical slice is only walls then at a wall)
    - Depth sensor for sure defines the top and bottom planes
- How do we interact with Motors?
- How do we ever get absolute positioning? Calc!!!

## 🛠 Solutions
- PIDs are used for the motors
    - Enter a position, measurement, set_point, opt velocity (override position), opt thrust (override velocity)
    - IMU can be used for position & angle
    - Measurement: Where you are
    - Set_Point: Where you want to be
    - Position: Hold Location (good for raw, pitch, roll)
    - Velocity: Hold Velocity (good for movement x, y, z)
    - Use Velocity to aim for a task and then hold position when at a good spot
- Provided two depths and the getting the angle of a pixel in a camera from the dead center of the camera
    - Sub is a guaranteed absolute depth from depth sensor
    - Lower sub to line up vertical center of camera with wanted item
    - Record depth
    - Rise back to any give depth and determine location with camera angle

## 📚 Resources
- [Team Handbook](https://robonation.gitbook.io/robosub-resources/section-3-autonomy-challenge/3.2-task-descriptions)
- [Task Ideas](https://robonation.org/app/uploads/sites/4/2025/02/Task-Ideas_RoboSub-2025.pdf)

## 🎯 Next Week’s Goals
- Review the defined states and clarify task responsibilities.
- Write more solid code for the states.

## 🔍 Additional Notes
- Navigating the Channel (Slalom) Task
    - Reverse line follower
    - Follow same side from gate task
    - Before task find depth via image recognition of red and - white boundary
    Keep white and red boundary in outer 1/4s of the camera
        - Use thickness of line as heuristic for distance
        - Use line follower to follow the line
        - Define state of accepted distance for navigated "to" slalom
        - Center on boundaries
        - Find next set of boundaries
        - Repeat
