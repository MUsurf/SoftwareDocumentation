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

## 🚧 Challenges
- Lack of clarity on task responsibilities
- Deciding Scope of State Machine

## 🛠 Solutions
-

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
