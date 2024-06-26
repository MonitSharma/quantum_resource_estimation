# Work with Q# Projects

With the release of the Azure Quantum Development kit, you can define Q# projects, which are folder strcutures with multiple Q# files that can access each other's resources. Projects are helpful for creating reusable libraries and logically organizing your source code.

A Q# project contains a Q# manifest file, named `qsharp.json` , and one or more `.qs` files in a specified folder structure. When a user opens a `.qs` file in VS code, or sets the `project_root` in a Jupyetr notebook or Python file , the compiler searches the surrounding folder hierarchy for the manifest file and determines the project's scope. If no manifest file is found, the compiler operates in a single file mode. A Q# project can be created manually or dirctly in VS code.


## A Q# project

A Q# project is defined by the presence of a `qsharp.json` manifest file and a **src** folder, both of which should be in the rootfolder of the project. For Q# programs, the Q# compiler detects the projects folder automatically. For Python and Jupyter users, you must specify the Q# project folder with `qsharp.init` call.

based on this repo, the root is `Azure_QRE`
```python
qsharp.init(project_root = '../Azure_QRE')
```


The folder strcutre for a Q# prjects remain the same.

![alt text](v2djm8xt.bmp)



## Create a Manifest file

A manifest file is a simple `.json` file named `qsharp.json` that can optionally include *author, license* and *.ints* fields. The minimum viable manifest file is the strings `{}`, which is autmatically created.

```python
{}
```

### Manifest File Examples


```python
{
    "author":"Microsoft"
}
```

or 

```python
{
    "author":"Microsoft",
    "license":"MIT"
}
```

