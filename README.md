# PoC of gRPC notifications - protobuf definition
Simple definition of NotificationService. The service defines two operations:

| Operation              | Description                                                                                |
|------------------------|--------------------------------------------------------------------------------------------|
| ping                   | The ping() operation accepts a unary request and returns a unary response.                 |
| serverSideStreaming    | The serverSideStreaming() operation accepts a unary request and returns a stream response. |
| bidirectionalStreaming | The bidirectionalStreaming() operation accepts stream and return stream response.          |

## Include protobuf definition into client/server project
In order to add `*.proto` files into client/server project you can use git submodule feature.

```
git submodule add git@github.com:jnicram/simple-notifications-proto.git notifications-proto
```

After adding a submodule you can generate necessary classes using a language-specific proto compiler.

Here more info: https://grpc.io/docs/protoc-installation/