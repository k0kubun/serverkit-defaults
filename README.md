# serverkit-defaults
[Serverkit](https://github.com/r7kamura/serverkit) plug-in for [defaults(1)](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/defaults.1.html) of Mac OS X.

## Resource
### defaults
Writes value for key in domain.

#### Attributes
- domain - defaults domain (default: `"NSGlobalDomain"`)
- key - defaults key (required)
- value - defaults value (required)

#### Example
```yml
resources:
  - id: autohide_dock
    type: defaults
    domain: com.apple.dock
    key: autohide
    value: 1
  - id: empty_dock
    type: defaults
    domain: com.apple.dock
    key: persistent-apps
    value: []
```
