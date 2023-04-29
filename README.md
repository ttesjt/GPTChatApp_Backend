# GPTChatApp_Backend
## The backend code for the chat app. Note this code is for AWS Lambda.  
## The frontend: https://github.com/ttesjt/GPTChatApp_Frontend

## 这个是gpt chat app 的后端代码，这份代码是为AWS Lambda专门提供的。
## 前端地址： https://github.com/ttesjt/GPTChatApp_Frontend


This is the backend code for my chatapp project. This backend is specifically for AWS lambda and S3 buckets. You will need to create the lambda function and S3 buckets on your own. Hopefully some code are reuseable for other service providers. You need to fill up the ./chat/documents/config.json file with your own api keys to use this backend.

这是一份后端代码。你需要对应的前端。这份代码需要你自行设置AWS lambda和S3 buckets。部分逻辑应该是通用的，但需要手动修改来适用于其他服务提供者。你需要在./chat/documents/config.json里填写你自己的api keys来让这个后端工作。

You will need to create 2 Lambda function in total. Both in Python 3.9. One should be names "Chat", and one should be named "User". Use the zip all files in "chat" folder for Chat Lambda. zip all files in "user" for User lambda. You will also need to create some S3 buckets. "multiversal-lovers-bucket", "m-lovers-character-bucket", "m-lovers-username-password-bucket", "multiversal-lovers-users-bucket", and "m-lovers-character-avatar-bucket".

您需要创建总共2个Lambda函数，都使用Python 3.9。一个应该命名为“Chat”，另一个应该命名为“User”。将“chat”文件夹中的所有文件压缩后用于创建Chat Lambda。将“user”文件夹中的所有文件压缩后用于创建User Lambda。您还需要创建一些S3存储桶。它们分别是："multiversal-lovers-bucket"，"m-lovers-character-bucket"，"m-lovers-username-password-bucket"，"multiversal-lovers-users-bucket"，以及"m-lovers-character-avatar-bucket"。
