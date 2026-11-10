# Anyrow Java SDK

[![MIT License](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)

Java client for the [Anyrow](https://anyrow.ai) extraction API, generated from its [OpenAPI spec](https://github.com/anyrow/openapi). Java 17 or later; its one dependency is Jackson.

## Install

Gradle:

```groovy
implementation 'ai.anyrow:anyrow-sdk:<version>'
```

Maven:

```xml
<dependency>
  <groupId>ai.anyrow</groupId>
  <artifactId>anyrow-sdk</artifactId>
  <version><!-- version --></version>
</dependency>
```

## Use

```java
import ai.anyrow.sdk.AnyrowClient;

AnyrowClient anyrow = AnyrowClient.builder()
    .baseUrl("https://api.anyrow.ai")
    .bearerToken(System.getenv("ANYROW_API_KEY"))
    .build();
```

Every API operation is a method on `AnyrowClient`; request and response types live in `ai.anyrow.sdk`. See the [API reference](https://anyrow.ai/docs) for what each one does.

## Other languages

[TypeScript](https://github.com/anyrow/sdk-typescript) · [Python](https://github.com/anyrow/sdk-python) · [Go](https://github.com/anyrow/sdk-go) · [Rust](https://github.com/anyrow/sdk-rust) · [C#](https://github.com/anyrow/sdk-csharp) · [CLI](https://github.com/anyrow/cli)
