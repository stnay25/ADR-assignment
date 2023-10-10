# ADR University network app

* Decision title: Performance Optimization 

* Status: Accepted 

* Deciders: Stadium Nay

* Date: 2023-10-07

* Context and Problem Statement:
The goal is to optimize the performance of the university social networking mobile app to ensure that the app will run smoothly on all sorts of devices.  

* Considered Options:
[1] Code splitting 
[2] Lazy Loading of Resources
[3] Progressive Web App
[4] Image Compression


* Decision:
The chosen performance optimization techniques are code splitting, lazy loading of resources, and image compression. This will ensure that the app runs smoothly on a wide range of devices. 

* Rationale:
The lazy loading of resources will reduce initial loading times and conserve bandwidth. This ensures that users who have slower connections or devices can still access content efficiently.

Code splitting will involve breaking the codebase on the app into smaller chunks that are loaded up only when needed. This will decrease the initial loading time and let the app perform better on devices with limited processing power. 

Image compression will reduce their file size while maintaining acceptable visual quality. This will benefit users who have lower-end devices by reducing data usage and increasing the speed of image loading. 
 
By implementing this technique, it will provide a smoother user experience across many spectrum of devices. 


* Consequences:
Implementing these techniques might require extra development effort in areas such as retrofitting them into the existing codebase. 
Rigorous testing is important to make sure that optimization will not create new problems or impact the user experience in a negative way. 
Regular maintenance is needed to update and fine-tune these optimization techniques as the app continuously gets upgraded and new specifications emerge for devices.


* Follow-Up Action:
The team will be responsible for implementing and putting in the code splitting, image compression, and lazy loading into the app codebase.

Much testing will be done to validate that the optimization doesn't hinder the functionality of the app.

Continuous monitoring of performance will be established to address any performance issues that may arise over time. Regular fine-tuning of optimization will be performed. 

Detailed documentation will be created to guide the development team in maintaining and updating the performance optimization 

Following this action will ensure that the university social networking app will keep performing optimally across many devices. 
