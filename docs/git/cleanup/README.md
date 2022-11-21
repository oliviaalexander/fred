## Cleanup

Deletes local and remote branches by the case number. If run without a casenumber, you will be prompted for one.

### Usage

```
Options:
      --version     Show version number                                [boolean]
  -h, --help        Show help                                          [boolean]
  -v, --verbose     Run with verbose logging                           [boolean]
  -c, --casenumber  Case number                                         [number]
```

### Example

```sh
fred git cleanup -c 1234
```