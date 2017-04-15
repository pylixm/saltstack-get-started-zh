# SaltStack 的灵活性

每个管理工具和他们的Git副本都声称是灵活的，但是当我们在SaltStack说灵活性时，我们的意思是整个管理方法的灵活性。

SaltStack可以实现为遵循最流行的系统管理模式：
- Agent and Server
- Agent-only
- Server-only
- 在同一环境中可混用上述模式

## AGENT AND SERVER

配置管理的标准模式。管理服务器向在大量系统上运行的代理发送命令和配置，并将结果返回给服务器。

## AGENT-ONLY

如果您不使用管理工具类功能，因为您不想设置所有这些“额外的东西”，这可能是您的模型。`Salt agents`可以在服务器或不涉及服务器的情况下执行管理任务。

这个模型最好的是它已经是内置的了;如果你不想使用管理服务器，你根本就不需要重新安装。您可以在此模型与`AGENT AND SERVER`模型之间来回切换，或将它们一起使用。

## SERVER-ONLY (AGENTLESS)

Salt命令可以使用SSH代替`Salt agent`在远程系统上执行。你可以使用`Salt Minion`配置所有Web服务器，也可通过SSH在数据库服务器上执行临时管理任务。

## NO SIZE FITS ALL

本“入门指南”的初步部分演示了使用代理和服务器模型的SaltStack来保证实例的简单性。如果您计划使用不同的方法，可以不使用这种方式。每个管理模型的主要区别是您使用的SaltStack可执行文件以及如何调用它。在开展工作时，每个模型的SaltStack功能基本相同。

## 主动和声明配置管理

SaltStack支持两种主要的方法来定义系统配置。遵循使用SaltStack强大的必备系统的声明式方法，或者采用内置有序执行的SaltStack的必要条件。