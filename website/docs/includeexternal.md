Evaluates a script, and marks any containers created by that script as external.

```lua
includeexternal("path")
```

For complex multi-workspace builds, it can be advantageous to have a set of projects that are generated by one workspace, and then used by the other workspaces as-is, without regenerating.

With this function, you can include a script which may contain one or more project or rule definitions. All such containers will be marked as external, and simply referenced, but not regenerated.


### Parameters ###

`path` is the file system path to a script file or a directory. See [include()](include.md) for a more complete description.


### Availability ###

Premake 5.0 or later.


### See Also ###

* [externalproject](externalproject.md)
* [externalrule](externalrule.md)
* [include](include.md)
