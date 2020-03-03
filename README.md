# Concierge - providing health and care computing and data services

Any health or care software application, whether for professionals or for patients, cannot work alone. 

It needs to interact with a wide range of different computing and data services, in order to operate safely and efficiently. Such applications, whether web-based or running on mobile devices, should be lightweight and ephemeral, focused on providing an outstanding user experience, and usually developed to solve a well-defined user need in a specific context, workflow or process.

To support such applications, Concierge provides a range of well-defined and easy-to-use, portable application programming interfaces, grouped into modular domain-driven services. 

1. Patient identity / demographics manager
2. Professional identity manager
3. Scheduling manager
4. Clinical document manager
5. Results and request manager
6. Clinical data manager
7. Reference data service
8. Terminology service

As a result, applications using Concierge are potentially portable across a range of health and care enterprises, relying on the underlying simple abstractions providing by the Concierge platform. Authentication and authorisation are an intrinsic part of the platform.

Concierge is a set of loosely-coupled *opinionated frameworks*. This means that many decisions are made explicitly on behalf of software developers working on client applications. Unopinionated frameworks can simply defer difficult decisions or force others to do hard work. For example, that means terminology binding is explicitly SNOMED CT with Concierge providing the appropriate mapping and integration if underlying services use an alternatively coding system. That means client applications see and process a harmonised, simpler view, hiding some of the complexities inherent in our health and care enterprises.

# What is provided?

Concierge services provide lightweight application programming interfaces (APIs), defined as gRPC services with a HTTP REST gateway. These gRPC definitions can be used to easily generate stub client or server implementations. 

Concrete implementations of Concierge services are currently heavily biased towards integrating with services within the National Health Service in Wales, UK. 
