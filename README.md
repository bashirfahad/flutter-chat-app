# Official Flutter packages for [Stream Chat](https://getstream.io/chat/sdk/flutter/)

![](https://raw.githubusercontent.com/GetStream/stream-chat-flutter/master/images/sdk_hero_v4.png)

[![CI](https://github.com/GetStream/stream-chat-flutter/actions/workflows/stream_flutter_workflow.yml/badge.svg?branch=master)](https://github.com/GetStream/stream-chat-flutter/actions/workflows/stream_flutter_workflow.yml)
[![Melos](https://img.shields.io/badge/maintained%20with-melos-f700ff.svg?style=flat-square)](https://github.com/invertase/melos)


**V4 Migration Guide**

> [!WARNING]
> Flutter `> = v3.16.x` uses material 3 by default which breaks the UI of some of the components.
> If you want to use these versions, you need to set the `useMaterial3` parameter to `false` 
> in the `ThemeData`.
>
> eg.
>
> ```dart
> MaterialApp(
>   theme: ThemeData(
>     useMaterial3: false,
>   ),
>   ...
> );
> ```
> 
> `StreamChat` widget overrides the `useMaterial3` parameter to `false` by default 
> so if you are using `StreamChat` widget, you **don't** need to set it manually.

For upgrading from V6 to V7, please refer to the [V4 Migration Guide](https://getstream.io/chat/docs/sdk/flutter/guides/migration_guide_7_0/)

## Sample apps and demos 
Our team maintains a dedicated repository for full fledged sample applications and demos. Consider checking out [GetStream/flutter-samples](https://github.com/GetStream/flutter-samples) to learn more or get started by looking at our latest [Stream Chat demo](https://github.com/GetStream/flutter-samples/tree/main/packages/stream_chat_v1). 

## Free for Makers

Stream is free for most side and hobby projects. To qualify your project/company needs to have < 5 team members and < $10k in monthly revenue.
For complete pricing details visit our [Chat Pricing Page](https://getstream.io/chat/pricing/)

## Structure
Stream Chat Dart is a monorepo built using [Melos](https://docs.page/invertase/melos). Individual packages can be found in the `packages` directory while configuration and top level commands can be found in `melos.yaml`. 

To get started, run `bootstrap` after cloning the project. 

```shell
melos bootstrap
```

## Packages 
We provide a variety of packages depending on the level of customization you want to achieve.

### [`stream_chat`](https://github.com/GetStream/stream-chat-flutter/tree/master/packages/stream_chat)
A pure Dart package that can be used on any Dart project. It provides a low-level client to access the Stream Chat service.

### [`stream_chat_persistence`](https://github.com/GetStream/stream-chat-flutter/tree/master/packages/stream_chat_persistence)
This package provides a persistence client for fetching and saving chat data locally. Stream Chat Persistence uses Moor as a disk cache.

### [`stream_chat_flutter_core`](https://github.com/GetStream/stream-chat-flutter/tree/master/packages/stream_chat_flutter_core)
This package provides business logic to fetch common things required for integrating Stream Chat into your application. The `core` package allows more customisation and hence provides business logic but no UI components.

### [`stream_chat_flutter`](https://github.com/GetStream/stream-chat-flutter/tree/master/packages/stream_chat_flutter)
This library includes both a low-level chat SDK and a set of reusable and customizable UI components.

### [`stream_chat_localizations`](https://github.com/GetStream/stream-chat-flutter/tree/master/packages/stream_chat_localizations)
This library includes a set of localization files for the Flutter UI components.

## Flutter Chat Tutorial

The best place to start is the [Flutter Chat Tutorial](https://getstream.io/chat/flutter/tutorial/).
It teaches you how to use this SDK and also shows how to make frequently required changes.

## Example Apps

Every package folder includes a fully functional example with setup instructions.

We also provide a set of sample apps created using the Stream Flutter SDK at [this location](https://github.com/GetStream/flutter-samples).

## Versioning Policy

All of the Stream Chat packages follow [semantic versioning](https://semver.org/).

See our [versioning policy documentation](https://getstream.io/chat/docs/sdk/flutter/basics/versioning_policy/) for more information.

