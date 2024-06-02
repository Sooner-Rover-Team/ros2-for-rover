# Actions - Long-Term Goals

An action is a type of interface that is used to start long-term activities, such as navigating to a waypoint, picking up an object, or anything else that can be described in terms of a goal.

Actions provide feedback on the progress of the action and provide the ability to cancel or preempt the action.

Action names define Actions, which look like a topic name but exist in a different namespace.

<!-- Give example of Action in REMI -->

## Parts of an Action

Action Client: the entity that requests an action, and waits for the action server to compute the sequence and return it, while receiving feedback.

Action Server: the entity that receives a request from an action client to start an Action. The action server then proceeds with the Action, providing feedback until finishing. Once it has finished, it returns a response to the action client.

## Creating an Action

To create an Action, we need to make a `.action` file inside the `action/` directory. These files have three fields: request, response, and feedback.

It takes the following format:

```IDL
int32 request
---
int32 response
---
int32 feedback
```
