# events-artifact

This is the artifact for [https://github.com/pythoneda-shared-artifact/events](https://github.com/pythoneda-shared-artifact/events "pythoneda-shared-artifact/events").

## How to declare it in your flake

Check the latest tag of the artifact repository: [https://github.com/pythoneda-shared-artifact/events-artifact-artifact/tags](https://github.com/pythoneda-shared-artifact/events-artifact-artifact/tags) and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-shared-artifact-events-artifact = {
      [optional follows]
      url =
        "github:pythoneda-shared-artifact/events-artifact-artifact/[version]?dir=events-artifact";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-shared-artifact-events-artifact-python38` 
- `#packages.[system].pythoneda-shared-artifact-events-artifact-python39` 
- `#packages.[system].pythoneda-shared-artifact-events-artifact-python310` 
- `#packages.[system].pythoneda-shared-artifact-events-artifact-python311` 

The Nix flake is under the 
[infrastructure](https://github.com/pythoneda-shared-artifact/events-artifact-artifact/tree/main/events-artifact "events-artifact") folder in <https://github.com/pythoneda-shared-artifact/events-artifact-artifact>.
