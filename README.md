# Protobuf
Learning about Protocol Buffers:
- Write simple and complex .proto files.
- Generate Code using `protoc`.
- Leverage Imports and Packages appropriately.
- Code in Python with Protocol Buffers.
- Understand advanced Protocol Buffers concepts.


## Chapeter 1: Introduction to Protocol Buffer

### Serialization vs Deserialization:
#### Human-Readable vs Computer-Readable Serialization

- When size matters (production) → prefer computer-readable (binary) formats like Protobuf. They are smaller, faster to serialize/deserialize, and cheaper to send over the network.

- When debugging/testing → prefer human-readable (text) formats like JSON or YAML, since developers can easily inspect and modify data.

- When configuration is user-facing → human-readable formats help with quick updates (editing a config file directly).

- When configuration is machine-facing → computer-readable formats are fine, especially if a UI acts as the middle layer.

👉 Rule of thumb:

- Use human-readable formats when humans need to read/edit the data directly.

- Use computer-readable formats when efficiency and performance are more important.
