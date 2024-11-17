# **Event_Driven_Architecture_project_02**
Event-driven architecture involves designing software systems where events trigger actions or workflows. In this setup, AWS S3, SQS, and Lambda work together to create an efficient and scalable event-driven solution.

# **S3 (Simple Storage Service):** 
  S3 is used to store files and data. When a new object is uploaded to an S3 bucket, it triggers an event.

# **SQS (Simple Queue Service)**: 
  SQS acts as a message queue to decouple the components of the system. The event triggered by the S3 upload is sent to an SQS queue, which ensures that the message is delivered to the       next component without being lost.

# **Lambda**: 
  AWS Lambda functions are triggered by the messages in the SQS queue. The Lambda function processes the event, performing actions such as data processing, transformation, or invoking other services.

Overall, this architecture ensures scalability and resilience by using S3 for storage, SQS for reliable message queuing, and Lambda for serverless, on-demand processing of events.


