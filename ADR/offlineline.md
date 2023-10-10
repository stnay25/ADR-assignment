# ADR University network app

* Decision title: Offline Mode Implementation

* Status: Accepted 

* Date: 2023-10-07

* Context and Problem Statement:
The task is to create an offline mode for a social media networking app for a university.  Any user should be able to access some features regardless if they have an internet connection or not. 

* Considered Options:
[1] Caching with background sync
[2] Local data storage with synchronization

* Decision:
The decision is to implement offline capabilities using the local data storage mechanism and data synchronization when the internet connection is accessible. Then use Redux offline as a framework that will manage the offline state and synchronize data with the server when it gets connected again. 

* Rationale:
Redux Offline allows the storage of relevant app data locally on the user's device, this makes sure that the user can access some features and data even if there is no internet connection.

Redux Offline has an established library with an active community, which means there is much access to documents, resources, and bug fixes. 

Redux Offline provides robust state management, this ensures that apps offline still run well enough.

When connection is available again, Redux Offline makes it easier for synchronization of data with the server, this ensures user data is up to date. 

* Consequences:
Even though Redux Offline has many benefits, it still needs some additional development to construct properly. So the team should ensure that data synchronization is well planned and any possible conflicts are handled. 

* Follow-Up Action:
The team will be responsible for creating and configuring redux Offline to handle any of the online data storage and synchronization effectively. 

Educate the user about the app's offline capabilities and how data synchronization works. 

Careful testing will be conducted to make sure offline mode works as it is supposed to. This includes testing many types of scenarios and conflicts. 

Taking this action will ensure that the offline mode implementation is successfully integrated into the social networking app for the university. 
