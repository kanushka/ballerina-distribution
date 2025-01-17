# Hello world

A GraphQL service in Ballerina represents a GraphQL schema. Each resource function of the `graphql:Service` represents a resolver function in the root `Query` type. The return type of each resource function will be the type of each field represented by the resource function.

For more information on the underlying package, see the [GraphQL package](https://lib.ballerina.io/ballerina/graphql/latest/).

This example shows a simple GraphQL endpoint that has a single field in the root Query type, which returns a string.

::: code graphql_hello_world.bal :::

Run the service by executing the following command.

::: out graphql_hello_world.server.out :::

Invoke the service as follows.

::: out graphql_hello_world.client.out :::
