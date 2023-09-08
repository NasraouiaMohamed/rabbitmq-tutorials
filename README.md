# RabbitMQ Tutorial - "Hello World!" with .NET

This tutorial demonstrates how to use RabbitMQ with .NET to build a simple messaging application.

## Introduction
In this tutorial, we will build upon the "Hello World!" example by creating a Work Queue. Work Queues are used to distribute time-consuming tasks among multiple workers efficiently. The main idea behind Work Queues is to avoid performing resource-intensive tasks immediately and instead schedule them for later execution. We encapsulate tasks as messages and send them to a queue, where worker processes running in the background will pop the tasks and process them. This approach is particularly valuable in scenarios like web applications where complex tasks cannot be handled within the short window of an HTTP request.