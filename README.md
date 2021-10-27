# cclp

Creative Commons License Placement Tool

```cmd
cclp kind=by-sa ver=3.0-unport name=LICENCE.md
```

key will be convert to LowerCase

key is as bellow.

- kind: required
  - desc: kind of license
  - choice: 6 of bellow, value will be convert to LowerCase
    - "by"
    - "by-sa"
    - "by-nd"
    - "by-nc"
    - "by-nc-sa"
    - "by-nc-nd"
- ver: optional
  - desc: version of license, value will be convert to LowerCase
  - default: latest-ver(now: 4.0)
  - regularize: 3.0 => 3.0-unport, 3.0-eu => 3.0-port
- name: optional
  - desc: file name, includes path to file.
  - default: LICENCE.md
  - regulaize: !(\.md) => \.md