# Dependency Injection with Unity
Using the Unity dependency injection container provides opportunities for you to more easily decouple components, business objects, and services you use in applications, and can simplify how you organize and architect these applications. This chapter provides overview of how Unity Container is initialized, used and disposed of in applications.
## The Dependency Injection Lifecycle: Registration, Resolution, Disposal
* [Registration](registration.md). With dependency injection, IoC container is responsible for injecting (pushing) the dependencies into the high-level client classes at runtime. In order for the container to perform the injection, types and all metadata (constructor, properties, fields, and methods), must be registered with the container. [Registration](registration.md) phase is when all these settings are intorduced to container.
* [Resolution](resolution.md). Once container configured it could be used to create and manage instances of types. During resolution it satisfies all dependencies in the way it was configured in registration phase. Once resolved instances are managed based on [lifetime](lifetime.md) specified during registration.
* [Disposal](disposal.md). Based on implemented interfaces and configuration container may dispose instances of created classes in several different ways. 