# KKU Metaverse – GitHub Project Content

Project URL: https://github.com/users/khamxay/projects/4  
Project Owner: khamxay  
Project Name: KKU Metaverse  
Main Work Package: KKU Virtual Campus Tour V1

---

## Recommended Project Fields

### Status
- Backlog
- Ready
- In Progress
- Review
- Testing
- Done

### Priority
- High
- Medium
- Low

### Workstream
- Proposal
- Unity Development
- 3D Assets
- UI/UX
- Audio Guide
- Testing
- Documentation
- Workshop Demo

### Sprint
- Sprint 1: Planning & Scene Setup
- Sprint 2: Waypoint System
- Sprint 3: UI & Audio
- Sprint 4: Assets & Route Completion
- Sprint 5: Testing & Optimization
- Sprint 6: Workshop Package

---

# Milestones

## Milestone 1: Proposal and Technical Planning
Goal: Prepare proposal, game flow, tour route, Unity structure, and development scope.

Deliverables:
- Proposal document
- Game Flow
- Campus Tour Route
- Scene Structure
- Timeline
- Acceptance Criteria

---

## Milestone 2: Unity Prototype V1
Goal: Build the first working prototype where avatar can visit 10 ordered checkpoints.

Deliverables:
- Unity scene: KKU_Campus_Tour
- PlayerAvatar
- NPC_Guide placeholder
- 10 waypoint objects
- WaypointTourManager.cs
- Popup information panel
- Progress tracking

---

## Milestone 3: Campus Content and Audio Guide
Goal: Add location descriptions, audio guide clips, and mission text.

Deliverables:
- Location name for each checkpoint
- Short description for 10 locations
- Audio guide for each point
- UI mission text
- Progress text

---

## Milestone 4: Testing and Workshop Demo
Goal: Prepare a stable version for workshop demonstration.

Deliverables:
- Functional testing
- Bug fixing
- Workshop guide
- User manual
- Developer manual
- Completion badge
- Final demo build

---

# Issues / Project Items

## Issue 1: Prepare KKU Virtual Campus Tour Proposal

**Type:** Documentation  
**Status:** Ready  
**Priority:** High  
**Workstream:** Proposal  
**Milestone:** Milestone 1

### Description
Prepare the full proposal for KKU Virtual Campus Tour V1. The proposal should explain the project background, objectives, scope, game flow, campus tour route, Unity scene structure, technical requirements, expected outputs, and development timeline.

### Tasks
- [ ] Write project background
- [ ] Define project objectives
- [ ] Define scope of Version 1
- [ ] Add 10 campus tour locations
- [ ] Add Game Flow
- [ ] Add Unity Scene Structure
- [ ] Add development timeline
- [ ] Add expected deliverables
- [ ] Add testing and acceptance criteria

### Acceptance Criteria
- Proposal is complete and readable
- Proposal includes both technical and workshop perspectives
- Proposal can be shared with project team or partner institution

---

## Issue 2: Create Unity Scene Structure

**Type:** Development  
**Status:** Ready  
**Priority:** High  
**Workstream:** Unity Development  
**Milestone:** Milestone 2

### Description
Create the main Unity scene for the KKU Virtual Campus Tour V1.

### Scene Structure
```text
KKU_Campus_Tour
├── PlayerAvatar
├── NPC_Guide
├── WaypointManager
├── UI_Canvas
│   ├── LocationPanel
│   ├── MissionText
│   └── ProgressText
├── Waypoints
│   ├── WP_01_Gate
│   ├── WP_02_Shrine
│   ├── WP_03_Lake
│   ├── WP_04_Convention
│   ├── WP_05_Registration
│   ├── WP_06_Dormitory
│   ├── WP_07_StudentDevelopment
│   ├── WP_08_Sports
│   ├── WP_09_KKUEnterprise
│   └── WP_10_HealthCenter
└── CampusBuildings
```

### Tasks
- [ ] Create Unity scene named `KKU_Campus_Tour`
- [ ] Add `PlayerAvatar`
- [ ] Add `NPC_Guide`
- [ ] Add empty object named `WaypointManager`
- [ ] Add parent object named `Waypoints`
- [ ] Create 10 waypoint empty objects
- [ ] Add `UI_Canvas`
- [ ] Create `LocationPanel`, `MissionText`, and `ProgressText`
- [ ] Create `CampusBuildings` parent object

### Acceptance Criteria
- Scene hierarchy follows the required structure
- All objects are correctly named
- Waypoints are ready to connect with script

---

## Issue 3: Implement WaypointTourManager.cs

**Type:** Development  
**Status:** Ready  
**Priority:** High  
**Workstream:** Unity Development  
**Milestone:** Milestone 2

### Description
Implement the waypoint tour logic using `WaypointTourManager.cs`. The script controls ordered campus tour progression, popup information, audio guide playback, progress text, and completion message.

### Tasks
- [ ] Create `WaypointTourManager.cs`
- [ ] Define `TourPoint` class
- [ ] Add `locationName`, `description`, `waypoint`, `audioGuide`, and `visited`
- [ ] Add player distance detection
- [ ] Trigger waypoint when player reaches checkpoint
- [ ] Show location panel
- [ ] Play audio guide
- [ ] Mark checkpoint as visited
- [ ] Unlock next waypoint
- [ ] Show completion message after final checkpoint

### Acceptance Criteria
- Player can trigger only the current waypoint
- Visited checkpoint is marked as completed
- Next waypoint unlocks after previous waypoint
- Progress text updates correctly
- Completion message appears after location 10

---

## Issue 4: Add 10 Campus Tour Locations

**Type:** Content  
**Status:** Ready  
**Priority:** High  
**Workstream:** Documentation  
**Milestone:** Milestone 3

### Description
Add the 10 ordered campus tour locations into the Unity project and documentation.

### Tour Route
1. University Gate
2. Mo Din Daeng Shrine
3. Si Than Lake
4. Golden Jubilee Convention Center
5. Registration Office
6. Dormitory Service Division
7. Student Development / Student Organization Building
8. Sports Division / Sports Center
9. KKU Enterprise
10. Student Health Center

### Tasks
- [ ] Add all 10 location names
- [ ] Add short description for each location
- [ ] Match each location with correct waypoint object
- [ ] Check order of tour route
- [ ] Confirm final checkpoint is Student Health Center

### Acceptance Criteria
- All 10 locations appear in correct order
- Each waypoint has name and description
- Route starts at University Gate
- Route finishes at Student Health Center

---

## Issue 5: Design UI Popup and Mission Progress

**Type:** Development  
**Status:** Ready  
**Priority:** High  
**Workstream:** UI/UX  
**Milestone:** Milestone 3

### Description
Create the UI system for showing location name, short description, mission text, progress text, and close button.

### Tasks
- [ ] Create `LocationPanel`
- [ ] Add `LocationTitleText`
- [ ] Add `DescriptionText`
- [ ] Add `MissionText`
- [ ] Add `ProgressText`
- [ ] Add close button
- [ ] Connect UI objects to `WaypointTourManager.cs`
- [ ] Test popup display at each checkpoint

### Acceptance Criteria
- Popup opens when reaching checkpoint
- Popup shows correct location name
- Popup shows correct description
- Mission text shows next location
- Progress text shows completed count
- Close button hides the popup

---

## Issue 6: Add Audio Guide System

**Type:** Development  
**Status:** Ready  
**Priority:** Medium  
**Workstream:** Audio Guide  
**Milestone:** Milestone 3

### Description
Add audio guide playback for each checkpoint using Unity AudioSource and AudioClip.

### Tasks
- [ ] Add AudioSource to WaypointManager or AudioManager
- [ ] Prepare audio guide clips for 10 locations
- [ ] Assign each clip to TourPoint
- [ ] Test audio playback at each checkpoint
- [ ] Stop or replace audio when moving to next checkpoint

### Acceptance Criteria
- Audio plays when checkpoint is reached
- Audio matches the correct location
- Audio does not overlap unexpectedly
- Audio system works in workshop demo

---

## Issue 7: Add Completion Badge

**Type:** Development  
**Status:** Ready  
**Priority:** Medium  
**Workstream:** UI/UX  
**Milestone:** Milestone 4

### Description
Create a completion badge shown after the player finishes the tour at the Student Health Center.

### Tasks
- [ ] Create completion panel
- [ ] Add badge graphic or icon
- [ ] Add message: `Tour Completed! Welcome to Khon Kaen University.`
- [ ] Show completion badge after location 10
- [ ] Hide mission text or change to completed state

### Acceptance Criteria
- Badge appears after final checkpoint
- Completion message is clear
- Player understands the tour is finished

---

## Issue 8: Workshop Testing and Bug Fixing

**Type:** Testing  
**Status:** Ready  
**Priority:** High  
**Workstream:** Testing  
**Milestone:** Milestone 4

### Description
Test the full KKU Campus Tour V1 for workshop readiness.

### Test Cases
- [ ] Player starts at University Gate
- [ ] NPC Guide mission text appears
- [ ] Checkpoint 1 triggers correctly
- [ ] All 10 checkpoints trigger in order
- [ ] Popup shows correct data
- [ ] Audio guide plays correctly
- [ ] Progress updates correctly
- [ ] Next waypoint unlocks correctly
- [ ] Completion badge appears
- [ ] Scene runs smoothly during workshop demo

### Acceptance Criteria
- No blocking bugs
- Tour can be completed from start to finish
- UI and audio work correctly
- Version is ready for workshop demonstration

---

## Issue 9: Prepare User Manual

**Type:** Documentation  
**Status:** Ready  
**Priority:** Medium  
**Workstream:** Documentation  
**Milestone:** Milestone 4

### Description
Prepare a simple user manual for workshop participants and project team.

### Tasks
- [ ] Explain how to start the tour
- [ ] Explain how to control avatar
- [ ] Explain how to follow mission text
- [ ] Explain how to read popup information
- [ ] Explain how to listen to audio guide
- [ ] Explain how to complete the tour
- [ ] Add troubleshooting notes

### Acceptance Criteria
- Manual is easy to understand
- Manual is suitable for workshop users
- Manual explains the complete tour flow

---

## Issue 10: Prepare Developer Manual

**Type:** Documentation  
**Status:** Ready  
**Priority:** Medium  
**Workstream:** Documentation  
**Milestone:** Milestone 4

### Description
Prepare developer manual for future improvement of KKU Campus Tour.

### Tasks
- [ ] Explain Unity scene structure
- [ ] Explain `WaypointTourManager.cs`
- [ ] Explain how to add new waypoint
- [ ] Explain how to edit location description
- [ ] Explain how to replace audio guide
- [ ] Explain how to adjust trigger distance
- [ ] Explain how to test the scene

### Acceptance Criteria
- Developer can understand the project structure
- Developer can update waypoints and content
- Developer can maintain Version 1 after workshop

---

# Timeline

## 6-Week Development Timeline

| Week | Main Activity | Output |
|---|---|---|
| Week 1 | Proposal and planning | Proposal, game flow, route, scene structure |
| Week 2 | Unity scene setup | Scene hierarchy, player, guide, waypoints |
| Week 3 | Waypoint script implementation | Working waypoint system |
| Week 4 | UI and audio guide | Popup, mission text, progress text, audio |
| Week 5 | Testing and optimization | Bug fixes, route testing, performance check |
| Week 6 | Workshop package | User manual, developer manual, final demo |

## Fast Sprint Timeline: 2 Weeks

| Day | Activity | Output |
|---|---|---|
| Day 1 | Confirm scope and route | Final route and feature list |
| Day 2 | Create Unity scene | Scene hierarchy |
| Day 3 | Create waypoints | 10 waypoint objects |
| Day 4 | Add script | WaypointTourManager.cs |
| Day 5 | Add UI | Popup and progress |
| Day 6 | Add descriptions | 10 location contents |
| Day 7 | Add audio | Audio guide clips |
| Day 8 | Test route | Functional checkpoint tour |
| Day 9 | Fix bugs | Stable prototype |
| Day 10 | Prepare demo | Workshop-ready version |

---

# GitHub Labels

Recommended labels:
- `proposal`
- `unity`
- `waypoint`
- `ui-ux`
- `audio-guide`
- `3d-assets`
- `testing`
- `documentation`
- `workshop`
- `high-priority`
- `medium-priority`
- `v1`

---

# README Section for Repository

## KKU Virtual Campus Tour V1

KKU Virtual Campus Tour V1 is an interactive Unity-based campus tour prototype for Khon Kaen University. The system allows an avatar to start at the University Gate and visit 10 important campus locations in order. At each checkpoint, the system displays the location name, short description, audio guide, and tour progress.

### Main Features
- Avatar starts at University Gate
- NPC guide explains the mission
- Ordered campus route with 10 checkpoints
- Popup information panel
- Audio guide at each checkpoint
- Progress tracking
- Completion badge at Student Health Center

### Tour Route
1. University Gate
2. Mo Din Daeng Shrine
3. Si Than Lake
4. Golden Jubilee Convention Center
5. Registration Office
6. Dormitory Service Division
7. Student Development / Student Organization Building
8. Sports Division / Sports Center
9. KKU Enterprise
10. Student Health Center

### Version
Version 1 is prepared for workshop demonstration.
