# Slim Behaviour Tree
## Table of Contents
  * [Demo](#Demo)
  * [Features](#Features)
  * [Examples of Usage](#Examples-of-Usage)
## Demo
Coming soon

## Features
* Basic node types included.
* Extendable. Custom nodes can be easily created.
* Blackboard to share data between nodes.
* Fluent builder
* More pre-built behaviors will be added <--- coming soon
* Gaphical Editor to view and edit trees <--- coming soon

## Examples of Usage
```
BehaviourTree tree = TreeBuilder.Init("testTree1", "JsonTest1")
                        .Selector().Do("TestAction1", TestAction1)
                                   .Condition("ConditionTest1", TestCondition1)
                                   .Do("TestAction2", TestAction2)
                        .End()
                        .Build();

tree.Run(new BaseInput());
```
