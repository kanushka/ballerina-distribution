# Subscriptions

A resource function with the `subscribe` accessor inside a GraphQL service represents a field in the root `Subscription` object type. Therefore, if a resource function with the `subscribe` accessor is present inside the Ballerina GraphQL service, the auto-generated schema will have a `Subscription` type.

Each resource function with the `subscribe` accessor in the service will be added as a field of the `Subscription` type. The field name will be the resource function name and the field type will be the constraint type of the stream returned from the resource function.

For more information on the underlying package, see the [`graphql` package](https://docs.central.ballerina.io/ballerina/graphql/latest/).

::: code graphql_subscriptions.bal :::

Run the service by executing the following command.

::: out graphql_subscriptions.server.out :::

Invoke the service as follows.

::: out graphql_subscriptions.client.out :::