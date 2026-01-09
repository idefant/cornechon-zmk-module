# Cornechon ZMK Module

## Usage

Edit your west.yml file found in your zmk-config's config directory to add the Cornechon module. Example:

```
manifest:
  remotes:
    - name: zmkfirmware
      url-base: https://github.com/zmkfirmware
    - name: idefant
      url-base: https://github.com/idefant
  projects:
    - name: zmk
      remote: zmkfirmware
      revision: v0.3.0
      import: app/west.yml
    - name: cornechon-zmk-module
      remote: idefant
      revision: v0.3.0
  self:
    path: config
```

Once you have the module added to your west.yml you can then build firmware as if it was in your config's shield directory or in ZMK main.
