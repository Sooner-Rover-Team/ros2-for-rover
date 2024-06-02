# Topics

Topics are one of three styles of [Interfaces](./interfaces.md). When [Nodes](./nodes.md) connect to topics, they use a publisher-subscriber (pub-sub) model. This means that Nodes can read data from a topic (by subscribing to it) and write data to a topic (by publishing to it). Topics can have one or more publishers and subscribers.

Topics should be used for continuous data streams, like sensor data.

Note: When a subscriber reads data from a topic, it does not know the publisher.

## Creating a Topic

We can describe the data of a Topic by creating a Message. Topics only store one message, and you can make one by creating a `.msg` file in the `msg/` directory of a ROS 2 package.

The following is an example of a message for a topic named `shapes/rectangle`:

```IDL
uint32 length
uint32 width 
```
