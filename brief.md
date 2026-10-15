Version: NAFATH-V2
Track: Networking
## Overview
To ensure critical emergency operations under high traffic, modern 5G networks are based on cloud-native microservices and virtualized slices. To deal with this structural complexity, operators use AI to forecast network overload and inform operational policies in advance of network service degradation. Cognitive mobile apps need to be built with a strong offline data synchronization feature to ensure uninterrupted functionality when connectivity is lost. In the meantime, 5G network slicing ensures individual low latency communication channels dedicated to emergency services. As distributed cloud architecture makes systems more susceptible to cyber attacks, strong cybersecurity countermeasures are applied throughout the incident response lifecycle to protect the systems against attacks. Last but not least, data engineering provides structured schemas for extracting operational metrics, which help admin optimise resources. Understanding how 5G network slicing can provide suitable network resources for emergency responders is essential for maintaining reliable communication during congestion and outages.

## Software
The HTTP methods GET, HEAD, OPTIONS, and TRACE are classified as "safe" methods, as their semantics are limited to read-only operations. PUT and DELETE are considered "idempotent" methods. These methods help prevent unintended duplicate actions or data corruption in the event of a connection issue, should the client attempt to repeat the operation.
Resource :RFC 9110-HTTP semantics-https://www.rfc-editor.org/info/rfc9110/#section-9.2.2.

## AI
Overfitting happens when a model is trained too much or too deeply into the training data, learning noise; the model then performs worse on new but unseen data. To prevent this, cross validation techniques like k-fold cross validation can be used by dividing the data into k folds and training and testing the model on different folds of the data. This will help the congestion-prediction model to perform better in real traffic conditions.
Resource:introducation to machine lerning with python-https://scikit-learn.org/stable/modules/cross_validation.html.

## Mobile
During an emergency, when a mobile application used by emergency response staff is no longer connected, it should be able to continue to function with a responsive user interface and store locally offline actions that occurred during the emergency in secure local storage. When network access is restored, a comprehensive data synchronization feature, which uses background queues, incremental data traffic, and conflict resolution algorithms, transfers all the information collected while offline, and seamlessly updates it on the central server without loss.
Resource:Apple developer docmention: corec data syncing-https://developer.apple.com/documentation/coredata.

## Networking
The software-defined networking (SDN) and network functions virtualization (NFV) technologies that underlie 5G network slicing enable the virtualization of logical networks that can be isolated from one another and operate on a common physical infrastructure. In emergency situations, the dedicated slices dynamically allocate guaranteed bandwidth and ultra-low latency only for first responders.This logical separation between public traffic and critical communications prevents severe public traffic congestion from impacting critical communications, ensuring no packet loss or traffic disruption to critical communications.
Resource:IBM think:what is 5G network slicing?-https://www.ibm.com/think/topics/5g-network-slicing.

## Cybersecurity
The incident response process has various phases, and the first phase is the preparation phase, where an organization aims to reduce the number of potential incidents by choosing and installing a series of security measures as part of a risk assessment. This is followed by the detection and analysis phase; since incidents can occur in countless ways, organizations must be generally prepared to handle any type of incident. The next phases are containment, threat eradication and recovery, though containment is essential to stop an incident from spreading, otherwise resources might be consumed or the damage could be extended. Finally, there are post-incident activities; all incident response teams need to evolve and adapt to meet the changing threats.
Resource:NIST SP 800-61 Rev.2:computer security incident handling guide-https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf

## Data
A star schema has a fact table at the center of the schema, which is directly linked to dimension tables like date and region. A snowflake schema decomposes dimensions into other related tables, it avoids the redundancy, but it will require more joins. A star schema is typically better for service-usage reporting, on the daily basis, due to the fact that it has a simpler schema that easier allows for analytical queries and reporting. Despite these, the operator should take into account the amount of data and reporting performance.
Resource:what is a schema? a complete guide to data modeling-https://www.snowflake.com/en/fundamentals/star-schema/.

## Misconception in My Track
One of the most prevalent misunderstandings about 5G network slicing is that each slice should have its own standalone physical network infrastructure. In fact, network slicing enables the formation of multiple virtual networks running on the same physical network and serving different service needs. For instance, an emergency response slice can be designed to be allowed to use critical communications without having to build an entirely new physical network. But, slicing doesn't ensure continuous service—appropriate resource management, monitoring and security are required.

## Open Question
How can predictive AI technologies seamlessly integrate with network slicing infrastructures to achieve self-allocation of resources in smart cities during major disasters without any human intervention?
