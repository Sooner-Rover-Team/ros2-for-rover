# Services

Services are a request/response communication, where the client (requester) is waiting for the server (responder) to make a short computation and return a result. They're a type of [Interface](./interfaces.md).

<!-- Give example of service in REMI -->

## Creating a Service

We can describe the form a service will take by creating a `.srv` file in the `srv/` directory in a ROS 2 package. They contain a request and response msg type, which is divided by `---`:

The following `.srv` describes a service that takes a string and returns a string:

``` IDL
string str  # Given fields
---
string str  # Returned 
```
