### Upload File Activity in UiPath Studio
This activity included in the ML Activities package sends the data from the RPA workflow to a given dataset. It connects to the AI Center tenant exactly in the same way as the ML Skill activity. We can then select the project and dataset in which we want to send the data back.

The Upload file activity has a new field called **Connection Mode.** Depending on the chosen **Connection Mode**, you can configure several essential properties directly from the body of the activity.

### Connection modes:
- **Connection Mode: Robot**
	1. Deploy the ML skill inside Robot.
- **Connection Mode: Endpoint**
	1. This allows our robot NOT to be connected to the same tenant.


The Upload File activity allows an RPA dev to select a project and a dataset path and send data back to the AI Center Datasets. This allows the model to continuously learn from new data.

UI path Orchestrator
- Orchestrator is the heart of your automation management. It give you the power to provision, deploy, trigger, monitor, measure, track and ensure the security of every robot in your organization. So now you can manage everything from your browser - or your mobile device.