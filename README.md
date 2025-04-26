# World-Weaver-Project-Guidelines
Please follow these guidelines as best as possible for organization. I don't care about the internals of the scripts, just make sure they make sense.

## 1. Naming Conventions
### General Rules:
* PascalCase for pretty much any created Instance in Explorer (Modules, scripts, folders etc)
* Try to use UPPER_SNAKE_CASE for any constants (not that necessary, just helpful).
* Please make sure the name makes sense for what it does. For example, if it is a service, try to include, 'Service' at the end of the module, or if it is a class that handles OOP, include 'er', 'manager' or 'controller' at the end. (SelectorController, TweenManager, LevelEditorController etc.)

## 2. Grouping & Organization
### Rule of Three:
If you have more than 3 similar objects, try to group them together. (Insert as a child, a folder etc)

### Function Grouping:
Try to group by function, not by object type.

## 3. Script Organization
### One script, one job:
Every script should have a clear responsibility, for example, 'AssetFunctions' module handles applying custom functions to objects, 'PaintSelector' strictly handles the paint UI

### DRY:
Try to follow the 'Don't-Repeat-Yourself' rule while coding. Same thing with modules, if there is a module that handles exactly what you need, use it, don't make a whole new module that does the same thing

### Modules:
We already do this, just make sure almost every logic is within a dedicated module

### Script location rules:
* Server logic: ServerScriptService
* Client logic: StarterPlayerScripts, StarterCharacterScripts, or within GUI
* Shared modules: ReplicatedStorage/SharedModules
* Try not to put scripts directly in ReplicatedStorage with no folder, or directly in Workspace.
* Make sure to insert the module if putting in ReplicatedStorage where it should belong.
* 3rd-Party library, please insert into 'Libraries'
* If the module isn't specific to something, insert it into Utilities

## 4. Avoid:
* Scripts named 'Script', 'LocalScript', 'ModuleScript'
* Mixing server and client code in the same location
* Deeply nested Instances (Some nesting is necessary for GUI)
