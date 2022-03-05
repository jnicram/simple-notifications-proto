# PoC of gRPC notifications - protobuf definition
Simple definition of NotificationService. The service defines two operations:

| Operation | Description                                                                   |
|-----------|-------------------------------------------------------------------------------|
| ping      | The ping() operation accepts a unary request and returns a unary response.    |
| notify    | The notify() operation accepts a unary request and returns a stream response. |