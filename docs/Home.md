# Tickets (Service Request) Classification - SAP Cloud for Customer extension
## Overview
This scenario is about streamlining service ticket processing using Machine Learning. Tickets (Service Request) are created in SAP Cloud for Customer (C4C) through the e-mail channel. Every Ticket creation triggers an extension on SAP Cloud Platform Extension Factory, Kyma Runtime which will extract the images attached to the e-mail and classify them using a Product Image Classification API from the SAP Leonardo Machine Learning Foundation - Functional Services. The best result will be mapped to the service request Object Category. This can be used to assign it to the right team/person for processing. By eliminating a manual classification step from the ticket routing procedure we can reduce the time to first (meaningful) response KPI significantly.
### Remark
This step-by-step guide is intended for hands-on session at SAP TechEd 2019. You can still follow the guide in an off-line mode by fulfilling the **Prerequisites** section below and then executing the **Process Steps**.

## Prerequisites
* You need to have an administrator access to a C4C system
* The email-to-ticket process should be enabled and configured in the C4C system.
* You need to have access to SAP C/4HANA Cockpit and you have provisioned a Kyma runtime ([documentation](https://help.sap.com/viewer/dbce7cc5e9e3469c84849d35e777fe0b/Current/en-US/363cf54bad2c47aeb44a87c215ad91ea.html)).
* You need to have access to SAP Leonardo Machine Learning Foundation - Functional Services.
* * We are using Product Image Classification API from SAP API Business HUB ([Link](https://api.sap.com/api/product_image_classification_api/resource)) in this sample.
* In real scenarios you need to train the SAP Leonardo Machine Learning Foundation - Functional Services in order to recognize the specific product categories intended.

## Process Steps
1. [Register and connect C4C system to Kyma runtime](https://github.com/SAP-samples/teched2019-C4C-CAA384/wiki/1.-Register-and-connect-C4C-system-to-Kyma-runtime).
1. [Develop, configure and deploy the Ticket Classification extension in Kyma runtime](https://github.com/SAP-samples/teched2019-C4C-CAA384/wiki/2.-Develop,-configure-and-deploy-the-Ticket-Classification-extension-in-Kyma-runtime).
1. [Test the Ticket Classification extension](https://github.com/SAP-samples/teched2019-C4C-CAA384/wiki/3.-Test-the-Ticket-Classification-extension).


***
[Next >](https://github.com/SAP-samples/teched2019-C4C-CAA384/wiki/1.-Register-and-connect-C4C-system-to-Kyma-runtime)