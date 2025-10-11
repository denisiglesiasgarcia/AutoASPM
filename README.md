# AutoASPM

A Python script that automatically activates ASPM for all supported devices on Linux.

It parses the `lspci -vv` output to determine which ASPM level is supported by
a device (e.g. L0s, L0sL1 or L1).

Forked from https://github.com/notthebee/AutoASPM to keep using the python version and not the nix new version.

### Dependencies

- pciutils
- python3

### Usage

```bash
sudo python autoaspm.py
```

### Credits

- Luis R. Rodriguez for writing the original enable_aspm script:
  https://www.uwsg.indiana.edu/hypermail/linux/kernel/1006.2/02177.html
- z8 for his Python rewrite of the enable_aspm script: https://github.com/0x666690/ASPM
- https://github.com/notthebee for re-rewriting it
