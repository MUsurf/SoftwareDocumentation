# SURF Software Weekly Updates Repository

Welcome to the **SURF Software Weekly Updates**! This repository is used to track the progress of software within SURF and act as a knowledge base for future use.

## 📌 Latest Weekly Reports
- [Team Webdev Weekly Update - 3/18](Spring-2025/Week-2/group-webdev-week-2.md)
- [Sim Weekly Update - 03/20/2025](Spring-2025/Week-2/group-sim-week-2.md)
- [Photon Ros Package Weekly Update - [3/18]](Spring-2025/Week-2/group-photon-week-2.md)
- [Team Motors Weekly Update - 3/18](Spring-2025/Week-2/group-motors-week-2.md)

## 📌 Purpose
Each week, teams should commit a write-up including:
- **Members**: Who contributed to this week's work?
- **Accomplishments**: What was completed this week?
- **Challenges**: Any obstacles faced?
- **Solutions**: How were issues resolved?
- **Resources**: Links to useful articles, research, or documentation.
- **Next Week's Goals**: What the team plans to focus on next.
- **Additional Notes**: Any other important updates.

## 🗂 Repository Structure
The weekly updates are organized by semester and week in the following format:
```
Season-Year/
    Week-#/
        group-name-week-#.md
```
Each group should create a markdown file for their updates and place it in the correct week's folder.

## 📝 How to Contribute
1. Navigate to the current semester's folder.
2. Open the appropriate week's folder.
3. Copy the template from `/templates/group-weekly.md`
3. Add your group's markdown file using the naming convention: `group-name-week-#.md`.
4. Commit and push your changes.

## 🔄 Automated Indexing
This repository includes an automation that updates this README to include direct links to all the latest weekly reports. The updated list of reports will be generated automatically.

## 🔄 Automated Folders
This repository includes an automation that adds the next weeks folder every monday as long as the last week had markdown files added. This is to limit the amount of work needed while ensuring it doesn't endlessly generate.

## TODO
- Fix Hardcoded Top Level Folder Name In Automations
- ~~Fix Always Creates New Week Folder~~
    - ~~Wanted Implementation: Only Create If Last Week Has Markdown~~
- ~~Prettier Automated Index By Grabbing First Line From File As Link Text~~
