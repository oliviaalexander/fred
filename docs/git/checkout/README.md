## Checkout

The checkout command reduces a few common GIT commands into one.  


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
fred git checkout -c 1234
```

### Addition info

This checkout command runs the following:

1. `git switch master`
2. `git pull`
3. `git checkout -b users/{username}/fb-{casenumber}`
4. `git push -u origin users/{username}/fb-{casenumber}`

If you do not provide the -c option followed by a case number, you will be prompted for one.

![checkout](./checkout-prompt.png)

The first time you run a command that requires a username for branch naming, you will be prompted for one.  It will be saved for future use and you will not be prompted again.

[Back](../README.md) to fred git documentation. 