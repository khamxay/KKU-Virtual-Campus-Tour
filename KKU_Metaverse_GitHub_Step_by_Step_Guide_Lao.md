# ຄູ່ມື GitHub Project ສໍາລັບ KKU Metaverse

**Project:** KKU Metaverse  
**GitHub User:** khamxay  
**Project Link:** https://github.com/users/khamxay/projects/4  
**Deadline:** 16/6/2026  
**Main Prototype:** KKU Virtual Campus Tour V1  

---

## 1. ຈຸດປະສົງ

ເອກະສານນີ້ເຮັດຂຶ້ນເພື່ອແນະນໍາຂັ້ນຕອນການນໍາຂໍ້ມູນໂຄງການ **KKU Virtual Campus Tour V1** ເຂົ້າໃນ GitHub Project ຊື່ **KKU Metaverse**.

ເປົ້າໝາຍຫຼັກຄືການຈັດການວຽກໃຫ້ທີມສາມາດເຮັດວຽກໄດ້ທັນກ່ອນວັນທີ **16/6/2026**.

---

## 2. ພາບລວມ Project

**KKU Virtual Campus Tour V1** ແມ່ນ prototype ໃນ Unity ສໍາລັບພາຜູ້ໃຊ້ເດີນທ່ຽວຊົມສະຖານທີ່ສໍາຄັນໃນ Khon Kaen University ຈໍານວນ 10 ຈຸດ.

### Main Features

- Avatar ເລີ່ມທີ່ University Gate
- NPC Guide ອະທິບາຍ mission
- ເດີນຕາມ waypoint 10 ຈຸດ
- ສະແດງ popup ຂໍ້ມູນແຕ່ລະສະຖານທີ່
- ມີ audio guide
- ມີ progress text
- ມີ completion badge ເມື່ອຈົບ tour

---

## 3. Campus Tour Route

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

---

## 4. Game Flow

```text
Start
↓
Welcome Screen
↓
Avatar Spawn at University Gate
↓
NPC Guide explains mission
↓
Visit 10 locations in order
↓
At each checkpoint:
  - Show location name
  - Show short description
  - Play audio guide
  - Mark as visited
  - Unlock next waypoint
↓
Finish at Student Health Center
↓
Show completion badge
```

---

## 5. Unity Scene Structure

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

---

## 6. ວິທີເຂົ້າ GitHub Project

1. ເຂົ້າເວັບ GitHub
2. Login ດ້ວຍ account `khamxay`
3. ເຂົ້າ link:

```text
https://github.com/users/khamxay/projects/4
```

4. ກວດຊື່ Project ໃຫ້ເປັນ:

```text
KKU Metaverse
```

---

## 7. ວິທີສ້າງ Item / Task ໃນ GitHub Project

1. ຢູ່ໜ້າ GitHub Project
2. ກົດປຸ່ມ **+ Add item**
3. ພິມຊື່ວຽກ
4. ກົດ **Enter**
5. ກົດເຂົ້າໄປໃນ item ເພື່ອໃສ່ description
6. ຕັ້ງ Status, Priority, Assignee, Sprint

---

## 8. ລາຍການ Task ທີ່ຄວນສ້າງ

```text
Prepare KKU Virtual Campus Tour Proposal
Create Unity Scene Structure
Implement WaypointTourManager.cs
Create 3D Campus Base Map
Create 10 Low-Poly Landmark Models
Design UI Popup and Mission Progress
Add Audio Guide System
Add Completion Badge
Workshop Testing and Bug Fixing
Prepare User Manual
Prepare Developer Manual
```

---

## 9. Recommended Project Fields

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

- Sprint 1: Setup and Planning
- Sprint 2: Unity + 3D Model
- Sprint 3: Integration and Testing
- Sprint 4: Final Demo

---

## 10. ຕົວຢ່າງການຈັດ Status

| Status | ວຽກ |
|---|---|
| Backlog | Future improvements, multiplayer, minimap |
| Ready | Proposal, Tour Route, Scene Structure |
| In Progress | 3D Model, Unity Scene, Waypoint Script |
| Review | UI, Description, Audio |
| Testing | Demo Route, Popup, Progress |
| Done | Final Demo, Manual, Workshop Package |

---

## 11. Milestones

### Milestone 1: Proposal and Technical Planning

**Goal:** ກຽມ proposal, game flow, route, scene structure, timeline.

**Deliverables:**

- Proposal document
- Game Flow
- Campus Tour Route
- Unity Scene Structure
- Timeline
- Acceptance Criteria

### Milestone 2: Unity Prototype V1

**Goal:** ສ້າງ prototype ທີ່ avatar ເດີນໄປ 10 checkpoints ໄດ້.

**Deliverables:**

- Unity scene
- PlayerAvatar
- NPC_Guide placeholder
- WaypointManager
- 10 waypoint objects
- WaypointTourManager.cs

### Milestone 3: 3D Assets and Campus Content

**Goal:** ສ້າງ 3D model ແບບ low-poly ແລະໃສ່ content 10 ຈຸດ.

**Deliverables:**

- Campus base map
- 10 low-poly landmarks
- Road/path
- Location descriptions
- Audio guide placeholders

### Milestone 4: Testing and Workshop Demo

**Goal:** ທົດສອບ ແລະກຽມ demo ໃຫ້ພ້ອມ.

**Deliverables:**

- Functional testing
- Bug fixing
- User manual
- Developer manual
- Final demo package

---

## 12. Issue Template: Create 3D Campus Base Map

```markdown
## Description
Create a simple 3D base map for KKU Virtual Campus Tour V1. The map should include basic terrain, road/path, landmark positions, and space for 10 campus tour checkpoints.

## Tasks
- [ ] Create simple terrain/base plane
- [ ] Add road or walking path
- [ ] Mark positions for 10 locations
- [ ] Export model to FBX or GLB
- [ ] Import into Unity
- [ ] Check scale and player movement

## Acceptance Criteria
- Campus base map is visible in Unity
- Avatar can move on the map
- Waypoints can be placed correctly
```

---

## 13. Issue Template: Create 10 Low-Poly Landmark Models

```markdown
## Description
Create simple low-poly 3D models for the 10 main KKU campus tour locations. The goal is to support workshop demonstration, not final realistic production.

## Landmark List
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

## Tasks
- [ ] Create simple model for University Gate
- [ ] Create simple model for Mo Din Daeng Shrine
- [ ] Create lake area for Si Than Lake
- [ ] Create simple convention center building
- [ ] Create registration office building
- [ ] Create dormitory service building
- [ ] Create student development building
- [ ] Create sports center building
- [ ] Create KKU Enterprise building
- [ ] Create student health center building
- [ ] Export all models to FBX or GLB
- [ ] Import models into Unity

## Acceptance Criteria
- All 10 landmarks are represented
- Models are lightweight and suitable for Unity/WebGL
- Names and positions match the tour route
```

---

## 14. Issue Template: Implement WaypointTourManager.cs

```markdown
## Description
Implement the waypoint tour logic using WaypointTourManager.cs. The script controls ordered campus tour progression, popup information, audio guide playback, progress text, and completion message.

## Tasks
- [ ] Create WaypointTourManager.cs
- [ ] Define TourPoint class
- [ ] Add locationName, description, waypoint, audioGuide, and visited
- [ ] Add player distance detection
- [ ] Trigger waypoint when player reaches checkpoint
- [ ] Show location panel
- [ ] Play audio guide
- [ ] Mark checkpoint as visited
- [ ] Unlock next waypoint
- [ ] Show completion message after final checkpoint

## Acceptance Criteria
- Player can trigger only the current waypoint
- Visited checkpoint is marked as completed
- Next waypoint unlocks after previous waypoint
- Progress text updates correctly
- Completion message appears after location 10
```

---

## 15. Issue Template: Design UI Popup and Mission Progress

```markdown
## Description
Create the UI system for showing location name, short description, mission text, progress text, and close button.

## Tasks
- [ ] Create LocationPanel
- [ ] Add LocationTitleText
- [ ] Add DescriptionText
- [ ] Add MissionText
- [ ] Add ProgressText
- [ ] Add close button
- [ ] Connect UI objects to WaypointTourManager.cs
- [ ] Test popup display at each checkpoint

## Acceptance Criteria
- Popup opens when reaching checkpoint
- Popup shows correct location name
- Popup shows correct description
- Mission text shows next location
- Progress text shows completed count
- Close button hides the popup
```

---

## 16. Timeline ຮອດ 16/6/2026

| Date | Unity Team | 3D Model Team | Output |
|---|---|---|---|
| 10/6/2026 | Setup GitHub Project, Unity scene | Confirm 10 landmarks and collect reference | Scope confirmed |
| 11/6/2026 | Create PlayerAvatar, WaypointManager, UI_Canvas | Create campus base map and road/path | Scene base ready |
| 12/6/2026 | Add WaypointTourManager.cs | Create model 1-4: Gate, Shrine, Lake, Convention Center | 4 landmarks |
| 13/6/2026 | UI popup and progress text | Create model 5-7: Registration, Dormitory, Student Development | 7 landmarks |
| 14/6/2026 | Add descriptions and audio placeholder | Create model 8-10: Sports, KKU Enterprise, Health Center | 10 landmarks |
| 15/6/2026 | Integrate all models into Unity and test route | Fix scale, position, texture, lighting | Prototype complete |
| 16/6/2026 | Final demo and documentation | Final export package | Workshop-ready V1 |

---

## 17. ການແບ່ງວຽກທີມ

| Role | Responsibility |
|---|---|
| Team Leader | Proposal, GitHub Project, Timeline, Final Demo |
| Unity Developer | Scene, waypoint system, UI, audio, build |
| 3D Modeler 1 | Base map, road/path, Gate, Shrine, Lake |
| 3D Modeler 2 | Convention, Registration, Dormitory |
| 3D Modeler 3 | Student Development, Sports, Enterprise, Health Center |
| Tester | Route testing, UI testing, bug report |
| Documentation | User manual, developer manual, README |

---

## 18. ມາດຕະຖານ 3D Model ສໍາລັບ V1

| Item | Standard |
|---|---|
| Style | Low-poly / simple clean model |
| Format | `.fbx`, `.glb`, or `.blend` |
| Texture | Simple color/material |
| Scale | Unity scale 1 unit = 1 meter |
| Naming | `KKU_01_Gate`, `KKU_02_Shrine`, ... |
| Collision | Box collider/simple mesh collider |
| Performance | Light enough for WebGL demo |

---

## 19. ໂຄງສ້າງ Folder ທີ່ຄວນມີໃນ Repository

```text
KKU-Metaverse
├── README.md
├── Documents
│   ├── Proposal
│   ├── Manual
│   └── Timeline
├── UnityProject
│   ├── Assets
│   ├── Scenes
│   └── Scripts
├── 3DModels
│   ├── Blender
│   ├── FBX
│   └── Textures
├── AudioGuide
│   ├── EN
│   ├── LA
│   └── TH
└── DemoBuild
```

---

## 20. ວິທີ Upload File ເຂົ້າ GitHub Repository

1. ເຂົ້າ repository
2. ກົດ **Add file**
3. ເລືອກ **Upload files**
4. ລາກໄຟລ໌ເຂົ້າໄປ
5. ຂຽນ commit message:

```text
Add KKU campus tour V1 project files
```

6. ກົດ **Commit changes**

---

## 21. ຖ້າໃຊ້ Git Command

### Clone Repository

```bash
git clone https://github.com/khamxay/KKU-Metaverse.git
```

### Enter Folder

```bash
cd KKU-Metaverse
```

### Check Status

```bash
git status
```

### Add Files

```bash
git add .
```

### Commit

```bash
git commit -m "Add KKU campus tour V1 project files"
```

### Push

```bash
git push
```

---

## 22. README.md ສໍາລັບ Repository

```markdown
# KKU Virtual Campus Tour V1

KKU Virtual Campus Tour V1 is an interactive Unity-based campus tour prototype for Khon Kaen University.

## Main Features
- Avatar starts at University Gate
- NPC guide explains mission
- 10 ordered campus checkpoints
- Popup information panel
- Audio guide
- Progress tracking
- Completion badge

## Tour Route
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

## Development Deadline
Final workshop-ready prototype: 16 June 2026
```

---

## 23. Final MVP Goal

ກ່ອນວັນທີ **16/6/2026** ໃຫ້ຈົບສິ່ງນີ້:

```text
Simple 3D Campus
+
10 Landmark Models
+
Waypoint Tour System
+
Popup Information
+
Progress Tracking
+
Completion Badge
+
Workshop Demo
```

---

## 24. Version 2 Ideas

ຫຼັງຈາກ workshop demo ສໍາເລັດ ຄ່ອຍພັດທະນາ:

- Realistic 3D buildings
- Better textures
- NPC animation
- Mini map
- WebGL optimization
- Multiplayer mode
- Mobile version
- Thai/Lao/English audio guide
