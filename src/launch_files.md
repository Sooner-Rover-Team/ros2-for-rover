# Launch Files

In ROS 2, you use Launch Files to start [Nodes](./nodes.md). You can write them in XML, YAML, or Python, and they're kept in the package's `launch/` directory. To start a ROS 2 project, there's typically one 'main' Launch File.

<!-- TODO(bray): define when it's appropriate to use each format. i prefer YAML (and maybe python, sometimes...) -->

## Functions

These files have several functions:

- Add command-line arguments.
- Import and run other Launch Files (including in other namespaces).
- Start a Node, setting its Namespace, and handing it the command-line arguments through its parameters.
  - You may also set "default" parameters in a Launch File if you expect people to type the same value often.
- Create Nodes to remap messages from one [Topic](./topics.md) to another.

## Example

Here's a short example that's using the YAML format.

```yaml
launch:

# TODO
```
