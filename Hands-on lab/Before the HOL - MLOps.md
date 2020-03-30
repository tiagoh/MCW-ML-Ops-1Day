![Microsoft Cloud Workshops](https://github.com/Microsoft/MCW-Template-Cloud-Workshop/raw/master/Media/ms-cloud-workshop.png "Microsoft Cloud Workshops")

<div class="MCWHeader1">
MLOps
</div>

<div class="MCWHeader2">
Before the hands-on lab setup guide
</div>

<div class="MCWHeader3">
November 2019
</div>


Information in this document, including URL and other Internet Web site references, is subject to change without notice. Unless otherwise noted, the example companies, organizations, products, domain names, e-mail addresses, logos, people, places, and events depicted herein are fictitious, and no association with any real company, organization, product, domain name, e-mail address, logo, person, place or event is intended or should be inferred. Complying with all applicable copyright laws is the responsibility of the user. Without limiting the rights under copyright, no part of this document may be reproduced, stored in or introduced into a retrieval system, or transmitted in any form or by any means (electronic, mechanical, photocopying, recording, or otherwise), or for any purpose, without the express written permission of Microsoft Corporation.

Microsoft may have patents, patent applications, trademarks, copyrights, or other intellectual property rights covering subject matter in this document. Except as expressly provided in any written license agreement from Microsoft, the furnishing of this document does not give you any license to these patents, trademarks, copyrights, or other intellectual property.

The names of manufacturers, products, or URLs are provided for informational purposes only and Microsoft makes no representations and warranties, either expressed, implied, or statutory, regarding these manufacturers or the use of the products with any Microsoft technologies. The inclusion of a manufacturer or product does not imply endorsement of Microsoft of the manufacturer or product. Links may be provided to third party sites. Such sites are not under the control of Microsoft and Microsoft is not responsible for the contents of any linked site or any link contained in a linked site, or any changes or updates to such sites. Microsoft is not responsible for webcasting or any other form of transmission received from any linked site. Microsoft is providing these links to you only as a convenience, and the inclusion of any link does not imply endorsement of Microsoft of the site or the products contained therein.

© 2019 Microsoft Corporation. All rights reserved.

Microsoft and the trademarks listed at <https://www.microsoft.com/en-us/legal/intellectualproperty/Trademarks/Usage/General.aspx> are trademarks of the Microsoft group of companies. All other trademarks are property of their respective owners.

**Contents**

<!-- TOC -->

- [MLOps before the hands-on lab setup guide](#mlops-before-the-hands-on-lab-setup-guide)
  - [Requirements](#requirements)
  - [Before the hands-on lab](#before-the-hands-on-lab)
    - [Task 1: Create an Azure Machine Learning workspace](#task-1:-create-an-azure-machine-learning-workspace)
    - [Task 2: Create a Compute Instance in your Azure Machine Learning workspace](#task-2:-create-a-compute-instance-in-your-azure-machine-learning-workspace)

<!-- /TOC -->

# MLOps before the hands-on lab setup guide

## Initial NOTICE

Please note that this instructions where modified to fit the 1 day remote workshop format. 

Feel free to check the original repo: https://github.com/microsoft/MCW-ML-Ops
## Requirements

1. Azure subscription. You will need a valid and active Azure account to complete the quickstarts. If you do not have one, you can sign up for a [free trial](https://azure.microsoft.com/en-us/free/).

   - The Microsoft Azure subscription must be pay-as-you-go or MSDN.

   - Trial subscriptions will not work. You will run into issues with Azure resource quota limits.

   - Subscriptions with access limited to a single resource group will not work. You will need the ability to deploy multiple resource groups.

2. Azure DevOps subscription. You will need a valid and active Azure DevOps account to complete the quickstarts. If you do not have one, you can sign up for a [free account](https://azure.microsoft.com/en-us/services/devops/).

   >**Note**: You will need privileges to create projects on the DevOps account. Also, you need privileges to create Service Principal in the tenet. This translates to `Ensure that the user has 'Owner' or 'User Access Administrator' permissions on the Subscription`.

3. Azure Machine Learning service workspace. We will be using a [Compute Instance](https://docs.microsoft.com/en-us/azure/machine-learning/concept-compute-instance) for the execution of the notebooks required for this workshop. See the instructions detailed below in order  to prepare your enviroment.

4. Azure Machine Learning service workspace. The workspace is created during Exercise 1 from the hands-on lab.

   >**Note**: Make sure you execute successfully all steps related to the Azure Machine Learning service workspace setup in Exercise 1. A correctly set up workspace is needed by all the other exercises.

## Before the hands-on lab

Duration: 5 minutes

For this workshop we will be using an Azure Machine Learning **[Compute Instance](https://docs.microsoft.com/en-us/azure/machine-learning/concept-compute-instance)** since it provides a fully-managed cloud-based workstation for data scientists.  

In the Compute Instance you will be able to execute the  required notebooks for this hands-on workshop.  

At a high level, here are the setup tasks you will need to perform to prepare your Compute Instance and enviroment (the detailed instructions follow):

1. Create an Azure Machine Learning workspace.

2. Provision a Compute Instance

3. Import the required notebooks for this workshop

### Task 1: Create an Azure Machine Learning workspace

1. In your browser, navigate to the [Azure Portal](https://portal.azure.com).

2. After sucesfull login with your corporate credentials, Click on **"Create Resource"**:

   ![Create Resource on Azure Portal](media/azure-portal-create-resource.png 'Create Resource')

3. Search for **"Machine Learning"** in the search input box (pick the first option as shown below):

   ![Search for Machine Learning](media/azure-portal-search-machine-learning.png 'Search for Machine Learning')

4. Click on **"Create"** in order to create the Azure Machine Learning workspace:

   ![Create Azure Machine Learning service](media/azure-portal-create-aml.png 'Create Azure Machine Learning')

5. Fill the details has described below.

   Please note:
   - For the "Workspace Name" replace the XXX by your name
   - Ask your proctor for the Resource group name to be used

   ![Create Azure Machine Learning service details](media/azure-portal-create-aml-workspace.png 'Create Azure Machine Learning service details')

6. The Azure Machine Learning workspace will be created and available for you shortly:

   ![Create Azure Machine Learning service creation](media/azure-portal-create-aml-workspace-creation.png 'Create Azure Machine Learning service creation')

### Task 2: Create a Compute Instance in your Azure Machine Learning workspace

1. In your browser, navigate to the [Azure Machine Learning portal](https://ml.azure.com).

2. Choose the workspace you created before:

   ![Choose Azure Machine Learning workspace](media/aml-portal-choose-workspace.png 'Choose Azure Machine Learning workspace')

3. Click on the left menu in the **Compute** section: 

![Azure Machine Learning - Choose Compute](media/aml-portal-create-compute.png 'Choose Azure Machine Learning compute')

4. Click on **"New"**:

![Azure Machine Learning - Create Compute Instance](media/aml-portal-create-computeinstance.png 'Azure Machine Learning Create Compute Instance')

5. Fill the details has shown below (note: provide any name that is suitable for you):

![Azure Machine Learning - Create Compute Instance details](media/aml-portal-create-ci-details.png 'Azure Machine Learning Create Compute Instance details')

6. After a few minutes your Compute Instance should be up and running: 

![Azure Machine Learning - Compute Instance running](media/aml-portal-ci-running.png 'Azure Machine Learning Create Compute Instance running')

7. Click on Jupyter (or JupyterLab):

![Azure Machine Learning - Jupyther](media/aml-jupyther-default.png 'Azure Machine Learning Jupyther')

8. Click on "New Terminal":

![Azure Machine Learning - Jupyther New Terminal](media/aml-jupyther-new-terminal.png 'Azure Machine Learning Compute Instance Jupyther Terminal')

9. Execute the following commands on the terminal:
 
 ```$ cd Users/```  
 ```$ ls ```  
 ```$ cd XXX``` (where XXX  is your username)  
 ```$ git clone https://github.com/tiagoh/MCW-ML-Ops-1Day```

 Below you seen the result of the execution of the previous commands: 

![Azure Machine Learning - Jupyther Commands](media/aml-jupyther-terminal-commands.png 'Azure Machine Learning Compute Instance Jupyther Commands')

10. Get back to the [Azure Machine Learning portal](https://ml.azure.com), select the **Notebooks** section. You should now see the contents of the previously cloned repository including the notebooks that we will be using later on the workshop:

![Azure Machine Learning - Notebooks](media/aml-notebooks.png 'Azure Machine Learning Notebooks')

You should follow all steps provided *before* performing the Hands-on lab.
