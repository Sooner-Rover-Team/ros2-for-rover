# Interfaces

An interface defines how Nodes communicate. They're comprised of different communication types:

- [Topics](./topics.md)
- [Services](./services.md)
- [Actions](./actions.md)

## Interface Definition Language (IDL)

Each of the three interfaces describes their fields in IDL, a language that tells [Nodes](./nodes.md) what to communicate.

### Fields

A field consists of two parts:

1. A data type: some 'kind' of data that's in some consistent form. See [the full list here](https://docs.ros.org/en/rolling/Concepts/Basic/About-Interfaces.html#field-types).
2. A name: any identifier.

These two combine to make the `datatype field_name` construct.

If we have a field: `string my_string`, it could store some text with the value "Hello world".

note: Fields can also have custom types made of [Messages] and their fields.

#### Default Values

Some data types can be [given default values](https://docs.ros.org/en/rolling/Concepts/Basic/About-Interfaces.html#field-default-value).
These look like a third part of the field, appearing after the field name:

<!-- TODO: check if bool is lowercase or uppercase -->

`bool field_name true`
