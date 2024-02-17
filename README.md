Introduction to the Bear Watch Instant Notification App
In this project you learn how to use platform events by building an instant notification app. With this application, park rangers can receive real-time notifications via the Salesforce platform.
![image](https://github.com/harika112003/Salesforce-Projects/assets/81819163/45902d1f-526f-4dc8-98d0-c3d2ee0c5071)


Screenshot showing home screen with an instant notification alert saying that bears have been sighted near the visitor center.

In the instant notification app that you build, events are published from a Heroku application via the REST API or from an Apex trigger on Chatter posts. Events are received by a Lightning console app that acts as a subscriber to the Event Bus via the lightning/empApi module. The following diagram illustrates this architecture.

Architecture diagram of the project.
![image](https://github.com/harika112003/Salesforce-Projects/assets/81819163/8d84d9a9-15a8-499f-8415-de52bc115ff0)

Overview of Platform Events
Platform events enable developers to deliver secure, scalable, and customizable event notifications. Events can be exchanged within the Salesforce platform or with external sources thanks to a publish-subscribe architecture. Apps can publish platform events by using Apex or one of the Salesforce platform APIs such as Pub/Sub, SOAP, REST or Bulk APIs. Flow can also publish platform events. Apps can subscribe to events in various ways: through Apex triggers, a Pub/Sub API (gRPC) client, a CometD client, the lightning/empApi module, or a Flow. CometD and gRPC are both HTTP-based event-routing protocols that enable external apps to subscribe to platform events without the need for polling. CometD is based on HTTP/1.1, whereas gRPC is based on the more modern HTTP/2 standard.
