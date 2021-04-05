# Google AI Platform 

This tutorial will cover the basics of creating a Jupyter notebook environment that will use Google Cloud Computing power to process large amounts of data. 

You must have a Google account and then must navigate to [Google AI Platform](https://cloud.google.com/ai-platform) and go to your AI platform console. 

## Create the Instance

- Press the "New Instance" button in the console and choose the type of pre-made environment you desire. Some environments come pre-installed with certain packages such as Tensorflow or SciKit Learn. Ensure to choose the environment that is best suited for your use case. 
- Select a name and select the desired region and zone. Tweak other parameters if necessary and then press create.

## Open the Jupyter Instance

- Navigate to the console and click on the "Open Jupyterlab". This will open up the Jupyter Notebook development environment. 

![](https://github.com/Samir-Sell/Cloud_Computing_Google/blob/main/Images/console.png)


## Change the Machine Type or add GPUs

- Once the testing phase of your workflow is completed. You will want to increase the amount CPUs and RAM your instance has available. This can be changed in a stopped instance. Navigate to your console and scroll in your instances to "Machine Type". You can then click the arrow to view the RAM and CPU options available. 
- If available in the zone and the environment, you can also add GPUs to your instance by looking under the column GPUs in your console. 

![](https://github.com/Samir-Sell/Cloud_Computing_Google/blob/main/Images/machine_type.png)

## Accessing data from Google Cloud Storage

- Ensure the bucket and the AI Platform instance are created in the same project as it will be easier to transfer information between the two services. Depending on your use case, there are multiple ways to access the data. 
- The different ways are specified [here](https://cloud.google.com/ai-platform/prediction/docs/working-with-cloud-storage#read-during-prediction). 
