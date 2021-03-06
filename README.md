
# **Predicting Customer Churn with Amazon SageMaker**

This lab is provided as part of **[AWS Innovate Data Edition](https://aws.amazon.com/events/aws-innovate/data/)**,  it has been adapted from an [AWS blog post](https://aws.amazon.com/blogs/machine-learning/predicting-customer-churn-with-amazon-machine-learning/)

Click [here](https://github.com/phonghuule/aws-innovate-data) to explore the full list of hands-on labs.
## Background

Losing customers is costly for any business.  Identifying unhappy customers early on gives you a chance to offer them incentives to stay.  This notebook describes using machine learning (ML) for the automated identification of unhappy customers, also known as customer churn prediction. ML models rarely give perfect predictions though, so this notebook is also about how to incorporate the relative costs of prediction mistakes when determining the financial outcome of using ML.

We use an example of churn that is familiar to all of us–leaving a mobile phone operator.  It seems like you can always find fault with my provider du jour! And if your provider knows that I’m thinking of leaving, it can offer timely incentives–you can always use a phone upgrade or perhaps have a new feature activated–and you might just stick around. Incentives are often much more cost effective than losing and reacquiring a customer.

## Setup: Launch AWS CloudFormation Stack

You will use AWS CloudFormation to deploy Amazon SageMaker in your AWS account. It will be deployed in the **Sydney region**. Please ensure you follow directions at the end of the lab to delete the CloudFormation stack to remove resources.

**1.** Login to your AWS account.

**2.** Right-click this link and open in a new browser tab: [Launch Stack into ap-southeast-2 with CloudFormation](https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-2#/stacks/new?stackName=SageMakerChurn&templateURL=https://s3-ap-southeast-2.amazonaws.com/aimlinnovate/sagemaker-churn-lab.yaml)

The CloudFormation console will be displayed, with some information already entered.

**3.** Click **Next** three times.

**4.** At the bottom of the page, select "I acknowledge that AWS CloudFormation might create IAM resources".

**5.** Click **Create stack**.

This will launch an Amazon SageMaker notebook instance. It will take approximately 3 minutes.

## Access SageMaker

**6.** In the **Services** menu at the top of the page, select **Amazon SageMaker**.

**7.** In the left navigation pane, click **Notebook instances**.

A SageMaker notebook instance will be displayed.

**8.** Click **Open Jupyter** in the right-hand column.

This will open a new browser tab to the Jupyter interface.

**9.** Click **lab_notebook.ipynb**.

This will open the notebook that will be used for the lab.

**Please follow the instructions in the notebook.** At the conclusion of the lab, please return the page you are currently reading to delete the CloudFormation template.

## Important: Clean-up

When you have completed the lab, you must delete the CloudFormation stack as follows:

**10.** Return to the AWS console and use the **Services** menu to go to **CloudFormation**.

**11.** Select the CloudFormation stack (click the circle).

**12.** Click **Delete**.

This will delete the stack and will stop charges being incurred in your AWS account.

## Survey
Please help us to provide your feedback [here](https://amazonmr.au1.qualtrics.com/jfe/form/SV_3a6rNirgLrWYRW6?Session=HOL01).
Participants who complete the surveys from AWS Innovate Online Conference - Data Edition will receive a gift code for USD25 in AWS credits. AWS credits will be sent via email by 30 September, 2021.
