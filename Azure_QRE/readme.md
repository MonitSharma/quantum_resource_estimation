# Work with Q# Projects

With the release of the Azure Quantum Development kit, you can define Q# projects, which are folder strcutures with multiple Q# files that can access each other's resources. Projects are helpful for creating reusable libraries and logically organizing your source code.

A Q# project contains a Q# manifest file, named `qsharp.json` , and one or more `.qs` files in a specified folder structure. When a user opens a `.qs` file in VS code, or sets the `project_root` in a Jupyetr notebook or Python file , the compiler searches the surrounding folder hierarchy for the manifest file and determines the project's scope. If no manifest file is found, the compiler operates in a single file mode. A Q# project can be created manually or dirctly in VS code.


## A Q# project


![alt text](v2djm8xt.bmp)