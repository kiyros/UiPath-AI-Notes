### About ML Skills
- An ML Skill is a live deployment of an ML Package. It can be used in an RPA workflow simply by dragging and dropping an ML Skill Activity in UiPath Studio.
- To view the list of ML Skills associated with a project, click the hotspots:
![[Pasted image 20220512150134.png]]


### Creating an ML Skill
1. Select ML Skills in the left side menu and then click on **Create New** from the top right corner. The **Create New ML Skill** Page will be shown.
2. An underlying ML Package along with its major and minor versions can be selected for deployment.
3. You can choose to enable GPU if it'll be available when the automation runs.

- When you create an ML skill, you need to select both the major and the minor version of the ML package
- You can update an existing ML skill to a new ML package version

### how to access a deployed ML skill in UiPath studio
- Connect to the same Orchestrator so the ML Skill is available to the Robot.
- Make the ML Skill Public and connect using endpoint, neither same orchestrator is needed nor same tenant nor same org
