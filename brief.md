Version: NAFATH-V2
Track: Networking
##Overview
To ensure critical emergency operations under high traffic, modern 5G networks are based on cloud-native microservices and virtualized slices. To deal with this structural complexity, operators use AI to forecast network overload and inform operational policies in advance of network service degradation. Cognitive mobile apps need to be built with a strong offline data synchronization feature to ensure uninterrupted functionality when connectivity is lost. In the meantime, 5G network slicing ensures individual low latency communication channels dedicated to emergency services. As distributed cloud architecture makes systems more susceptible to cyber attacks, strong cybersecurity countermeasures are applied throughout the incident response lifecycle to protect the systems against attacks. Last but not least, data engineering provides structured schemas for extracting operational metrics, which help admin optimise resources. All these interwoven technologies are integral to the system as a whole and help keep 5G emergency services resilient during stress.

##Software
The HTTP methods GET, HEAD, OPTIONS, and TRACE are classified as "safe" methods, as their semantics are limited to read-only operations. PUT and DELETE are considered "idempotent" methods. These methods help prevent unintended duplicate actions or data corruption in the event of a connection issue, should the client attempt to repeat the operation.
Resource :RFC 9110-HTTP semantics-https://www.rfc-editor.org/info/rfc9110/#section-9.2.2.

##AI
Overfitting happens when a model is trained too much or too deeply into the training data, learning noise; the model then performs worse on new but unseen data. To prevent this, cross validation techniques like k-fold cross validation can be used by dividing the data into k folds and training and testing the model on different folds of the data. This will help the congestion-prediction model to perform better in real traffic conditions.
Resource:introducation to machine lerning with python-https://scikit-learn.org/stable/modules/cross_validation.html.

##Mobile
During an emergency, when a mobile application used by emergency response staff is no longer connected, it should be able to continue to function with a responsive user interface and store locally offline actions that occurred during the emergency in secure local storage. When network access is restored, a comprehensive data synchronization feature, which uses background queues, incremental data traffic, and conflict resolution algorithms, transfers all the information collected while offline, and seamlessly updates it on the central server without loss.
Resource:Apple developer docmention: corec data syncing-https://developer.apple.com/documentation/coredata.

Networking

Cybersecurity

Data

Misconception in My Track

Open Question
