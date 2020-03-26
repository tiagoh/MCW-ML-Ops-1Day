# Before you start - IMPORTANT NOTICE

This repository is a fork of the following Github repository: https://github.com/microsoft/MCW-ML-Ops

All the content available in this repo (and specially all the credits!) is based on the exising "Microsoft Cloud Workshop - MLOps" available on its original source.

We have simply modified slightly the agenda, structure and some content to tailor it into a 1 day workshop.

**Agenda**: 

*09:00 - 11:30* Presentation and Demo  
Introduction to Azure Machine Learning, brief overview, key features and MLOps  
Architecture E2E for Machine Learning and MLOps

*11:30 - 13:30* Personal Time / Lunch break
 
*13:30 - 16:30* Hands-on Lab (self paced)  
Possibly ad-hoc meeting to discuss common problems during lab execution  
Questions can be asked in Teams chat  
Individual calls with the proctors if needed during this time  
 
*16:30 - 17:00* Wrap-up and Q&A

**Note:** *Whiteboard design session was removed due the remote nature of the workshop. You can still see the content in the `original_unused\Whiteboard design session` folder*

# MLOps

Trey Research Inc. delivers innovative solutions for manufacturers. They specialize in identifying and solving problems for manufacturers that can run the range from automation, to providing cutting edge approaches that generate new opportunities. Trey Research has decades specializing in data science and application development that until now were separate units. They would like to unlock the greater, long term value by combining the two units into one, and follow one standardized process for operationalizing their innovations.

For this first proof of concept (PoC), Trey Research Inc. are looking to leverage Deep Learning technologies with Natural Language Processing (NLP) techniques to scan through vehicle component descriptions to find compliance issues with new regulations. The component descriptions are managed via a web application, and the web application takes the description and labels the component as compliant or non-compliant using the trained model. As part of this PoC, they want to ensure the overall process they create enables them to update both the underlying machine learning model and the web app in one, unified pipeline. They also want to be able to monitor the model's performance after it is deployed so they can be proactive with performance issues.

November 2019

## Target audience

- Data Scientists
- App Developers
- AI Engineers
- DevOps Engineers

## Abstracts

### Workshop

In this workshop, you will learn how Trey Research can leverage Deep Learning technologies to scan through their vehicle specification documents to find compliance issues with new regulations, and manage the classification through their web application. The entire process from model creation, application packaging, model deployment and application deployment needs to occur as one unified repeatable, pipeline.

At the end of this workshop, you will be better able to design and implement end-to-end solutions that fully operationalize deep learning models, inclusive of all application components that depend on the model.

### Presentation and Demo

This presentation gives a gentle introduction to Azure Machine Learning by providing a brief overview of some key capabitilies before diving into MLOps.  

It then gets into more detail on the typical E2E scenario of a Machine Learning project by providing a reference architecture for MLOps.  

The discussed process and architecture is tipically used on Production scenarios across many Enterprise customers.

The presentation deck is available in the `Presentation` folder

### Whiteboard design session

**Note**: *This section is not in the workshop agenda due the remote nature. We have kept this section for further reference and the contents on the `original_unused\Whiteboard design session` folder*

In this whiteboard design session, you will work in a group to design a process Trey Research can follow for orchestrating and deploying updates to the application and the deep learning model in a unified way. You will learn how Trey Research can leverage Deep Learning technologies to scan through their vehicle specification documents to find compliance issues with new regulations. You will standardize the model format to ONNX and observe how this simplifies inference runtime code, enabling pluggability of different models and targeting a broad range of runtime environments and most importantly improves inferencing speed over the native model. You will design a DevOps pipeline to coordinate retrieving the latest best model from the model registry, packaging the web application, deploying the web application and inferencing web service. You will also learn how to monitor the model's performance after it is deployed so Trey Research can be proactive with performance issues.

At the end of this whiteboard design session, you will be better able to design end-to-end solutions that will fully operationalize deep learning models, inclusive of all application components that depend on the model.

### Hands-on lab

In this hands-on lab, you will learn how Trey Research can leverage Deep Learning technologies to scan through their vehicle specification documents to find compliance issues with new regulations. You will standardize the model format to ONNX and observe how this simplifies inference runtime code, enabling pluggability of different models and targeting a broad range of runtime environments and most importantly, improves inferencing speed over the native model. You will build a DevOps pipeline to coordinate retrieving the latest best model from the model registry, packaging the web application, deploying the web application and inferencing web service. After a first successful deployment, you will make updates to both the model, the and web application, and execute the pipeline once to achieve an updated deployment. You will also learn how to monitor the model's performance after it is deployed so Trey Research can be proactive with performance issues.

At the end of this hands-on lab, you will be better able to implement end-to-end solutions that fully operationalize deep learning models, inclusive of all application components that depend on the model.

## Azure services and related products

- Azure Container Instances
- Azure DevOps
- Azure Kubernetes Service
- Azure Machine Learning Service
- Azure Notebooks
- ML Ops
- ONNX
  
## Related references

- [MCW](https://github.com/Microsoft/MCW)

## Help & Support

Please refer to the original repository: https://github.com/microsoft/MCW-ML-Ops