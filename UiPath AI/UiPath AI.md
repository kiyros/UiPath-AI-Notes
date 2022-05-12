

## four main concepts related to artificial intelligence



### Where do RPA and AI meet?
- RPA has already proven its value by helping customers automate rule-based and repetitive tasks throughout an organization.
- However, a significant part of the work cannot be easily tackled by traditional RPA. We're talking about sophisticated work involving cognitive tasks, such as classifying emails and predicting sales. This is where AI comes into play and takes RPA to the next level.
- When conceptualizing RPA and AI, it can be helpful to think of AI as the brain, and RPA as the hands. A disconnected brain can dream up concepts, but without hands, it's impossible to apply them. At the same time, it's impossible to handle advanced processes without a brain. It's when the two are combined that complex tasks can be accomplished.
- This is the place for [[Identifying Use Cases]] for AI Center where you can automate more by adding AI to your automation.


### AI (Artificial Intelligence)
- AI
	- Development systems that are able to preform tasks that normally require human intelligence and decision making.
- Machine Learning (ML)
	- a sub-field of AI that enables system to learn from data. Systems learn from previous experience and information to deduce and predict future info.
	- To do this they use algorithms that learn to perform a specific task without being explicitly programmed.\
- Deep Learning (DL)
	- An area of machine learning concerned with Artificial neural networks.
	- These are a series of algos that aim to recognize relationships in a set of data through a process that mimics biological neural networks
- Natural Language Processing (NLP)
	- A branch of AI that deals with understanding and generating human languages.
- Computer Vision
	- A field of AI that enables computers to gain high-level understanding from digital images or videos.
	- AI = brain, then computer vision is the eye that enables the computer to observe and understand. like the human eye.

![[Pasted image 20220502232953.png]]


## Closer look at machine learning

#### what is the objective of a machine learning algorithm?
- input -> function -> output
- __input__ : could be training data such predicting housing prices, the input would be size, number of bedrooms, neighborhoods, schools and hospitals around. this serves as training data.
- __function__: predicts the housing prices from the input data. The training data teaches out ML models.
- __output__: By processing the input data, the algorithm would model the house prices and would be able to predict the output - the price of a given house.

#### How does machine learning work?
- ML: is about computers trying to learn from experience.
- A computer program is trying to solve a problem by making a prediction, model or understanding what the program is looking at. Expierence means the computer program learns from many examples. These examples include more data leading to more questions hence, better answers.

![[Pasted image 20220502234617.png]]
- __data:__  we need to train the machine model by using training datasets.
- __Creating a model__: Given a set of data or observations, we try to fit a function to it. once finished we are ready to make predictions on new data.
- __Make a prediction__: the model predicts the output based on the given inputs.
- __feedback loop__: After the first training cycle, we won't fully know the form of the function. Its important to keep retraining the model by feeding it with new data and providing human feedback on the accuracy of the outcomes.

#### Types of Machine learning
##### Supervised learning
- in supervised learning, algorithms map the input variables with the output variables. In every case there is a correct answer, so the aim is to train the model until it reaches an acceptable level of performance in predicting the outcome, at which point the learning stops.
- there are 2 types of problems solved by this method
	- __classification__: the output variable is a category (red or blue, yes or no, spam or no spam)
	- __regression__: The output variable is a real value (amount, weight).

##### Unsupervised learning
- In this model there are only input variables, but no corresponding output variables. The goal of the algorithm is to model the underlying structure of the data, but no correct answer and no teachers.
- But there are 2 problems:
	- Clustering: Inherent groupings of data, such as credit card transactions to identify outliers, potentially indicating frauds;
	- Association: correlations between data, such as people that buy X also buy Y.

##### Reinforcement Learning
- Algorithms try to solve a problem in an uncertain, potentially complex environment only by trial and error and using a system of rewards and punishments. There are no correct answers, but feedback is given in the form of rewards and penalties.

- Consider the example of a robot trying to learn how to shoot a basketball. Each time the ball goes in the basket the robot realizes it did something good and remembers what it did. Each time it misses, it learns from that information as well.


### How do you decide which machine learning algorithm to use?
- Deciding which algorithm to use can seem overwhelming. There are a lot of machine learning algorithms and each takes a different approach to learning. There's no universal option available. Choosing an algorithm is just trial and error.  Even an experienced data scientist cannot tell whether an algorithm works without trying it out.
- Algorithm selection depends on the size and type of data you are working with. It depends on the understanding you want to get from the data.
- Here are 2 tips:
	- Choose **Supervised Learning:** if you need to train the model to **make a prediction**, for example-the future value of a stock price. Or, if you need to train the model to **make a classification**, for example-given a handwritten character, classify it as one of the known characters.
	- Choose **Unsupervised Learning:** if you need to explore the data and train the model to find hidden data as well as draw inferences from the datasets. For example-grouping images based on pattern recognition, inventory management for stores selling thousands of products per month.
![[Pasted image 20220503012502.png]]


###  What Is AI Center?
 - it is an application that enables deploying, consuming, managing, and improving machine learning models.
 - It can manage models built by in-house data scientists, by UiPath and our partners, and even open-source models.
 ![[Pasted image 20220503200026.png]]
 - choosing a model:
	 - supports the ML models you build
	 - Offers access to out-of-the-box models from UiPath, from UiPath technology partners or open-source models from the community.
- AI center:
	- Once a model is uploaded from out-of-the-box options, it can be trained, managed and consumed through an ML skill.
- ML skill:
	- The skills created in AI center using ML packages can be easily put to work in RPA workflows in UiPath Studio, where decisions are made.
- Humans:
	- In case the decisions made by robots using the ML skills deployed return LOW confidence levels, the human user can be involved to offer feedback and validate the results.
- Improve models based on human validated data
	- The RPA workflows can be built to send the data in automations to retrain the ML models in AI center. This includes the outcomes of the human input.


### Types of machine learning models on AI Center
- **Bring Your Own Model**: models built by your data science team.
- **Open-source model**: models built by the data scientist community. Customers will be able to manage them in AI Center and train and deploy them directly in the RPA workflows.
- **Pick a model**: models built by UiPath technology partners.
- **Out-of-the-box models**: pre-built models supported by UiPath.

### Who uses AI Center?
- Data scientist:
	- Building and uploading the ML models to AI Center.
- Process Controller:
	- improving the ROI of automations by deploying models already uploaded by Data Scientists or provided by UiPath into ML skills.
- RPA Developer:
	- Consuming the available ML skills within customized RPA workflows where decisions are made by the robots.


### What are Various ways to deploy AI Center?
1.) **In Cloud Availability**
- In this setup, AI Center is available as a service hosted in UiPath cloud. UiPath manages all the necessary product infrastructure, including the machine learning models, and is fully responsible for making sure everything functions correctly.
- Features:
	- Deploy, manage, and improve ML models on UiPath Automation Cloud.
	- Requires no infrastructure and no maintenance
	-   Uptime guarantee for the enterprise version.
	-   Frequent patches are released with new features and bug fixes, under the Automation Cloud release cadence.
	-   Document Understanding metering is done in UiPath cloud.
	-   Internet access is required.

2.) **On-premises Air-gapped**
- Air-gapped installation allows customers to use AI Center in a disconnected environment, when there is no internet connection to reach UiPath licensing server. This means that at both install time and runtime, no outbound connections are needed to use a fully-featured version of AI Center.
- Air-gapped is popular among our customers in public and financial services sectors, which have highly secure environments.
- **No internet access is required.**

3.) **On-Premises Online**
- AI Center is deployed in the customer's infrastructure, either on a local server or on their private cloud. Customers take control over hosting their machine learning models.
- **Features:**
	- Deploy, manage, and improve ML models locally.
	-   Customer-managed infrastructure.
	-   Fully integrated with on-premises Orchestrator.
	-   Releases patches with a much slower cadence.
	-   Easy installation due to the automatic retrieval of the installer and associated artifacts from the internet.
	-   Easy management, as updates to AI Center and/or models can be automatically downloaded.
	-   Document Understanding metering is done in UiPath cloud.

4.) **Hybrid Mode (Cloud AI Center + Orchestrator on-premise)**
-   Robots can be connected to the on-premises Orchestrator.
-   Robots can call ML Skills to upload data to a dataset.
-   Calling of ML Skills can be done by using the new ML Services activities along with the Public ML Skills and Public datasets features.
-   Allows customers to benefit from ALL of the advantages of AI Center in the cloud, without having to migrate their existing on-premises Orchestrator.
-   Frequent patches with new features and bug fixes, under the cloud platform release cadence.
-   No requirement for installation and management on the AI Center.
-   Document Understanding Metering is done in UiPath cloud.
-   Internet access is required.

5.) **Automation Suite**
-   Automation Suite enables you to deploy the full UiPath Automation Platform in the environment of your choice, including bare metal machines, on-premises Virtual Machine infrastructure, or cloud subscriptions to any of the major providers.
- Automation Suite contains everything in one package that you can deploy in multi-node mode with automatic scaling and built-in HA, monitor, configure, and upgrade.
-   Deployment profiles must be chosen accurately. To know more about deployment architecture, requirements, and installation, check [this](https://docs.uipath.com/automation-suite/docs/deployment-architecture-and-installation-best-practices) link.


### Types of AI Center On-Premises Online Installation
- Single - Node installation: 
	- AI Center can be deployed on any physical or virtual machine. The AI Center installer also includes the installation of Kubernetes on the machine.
- Multi - Node Installation:
	- This new feature lets customers run many ML Skills and training pipelines in an environment with high-availability and scalable processing power. 
	- AI Center on multi-node bundled Kubernetes deploys AI Center in multi-node configuration. It is recommended to install it on fresh cloud virtual machines in Azure, AWS or GCP. Azure Kubernetes Service is also supported, as well as bare-metal installations.


### An End-to-End Preview of AI Center
-   Describe the process of creating ML projects in AI Center, uploading datasets and training ML packages, deploying them as ML skills in RPA workflows in Studio and configuring the feedback loop with AI Center.
-   Define the concepts related to AI Center - Projects, Datasets, Data Labeling, ML packages, Pipelines, ML skills, and ML logs.

#### Let's look at the context
A motor insurance company has a dedicated "Motor Insurance folder" to receive vehicle insurance claims from policyholders. The vehicles are bikes, cars, and buses. The priority of the company is the speed of providing insurance to each claim. 

The motor insurance company decides to automate the process of classifying emails and placing them into dedicated folders, from where specialized teams can focus their effort on solving them. This is what the process will look like.![[Pasted image 20220503233609.png]]
![[Pasted image 20220510133251.png]]
