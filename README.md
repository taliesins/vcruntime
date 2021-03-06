Microsoft Visual C++ Runtime Cookbook
=====================================

[![Cookbook Version](https://img.shields.io/cookbook/v/vcruntime.svg)](https://supermarket.chef.io/cookbooks/vcruntime)


Installs Microsoft Visual C++ runtime version 9 (2008), 10 (2010) or 12 (2012) on Windows.

Requirements
------------
#### Platforms
* Microsoft Windows 2008 R2
* Microsoft Windows 2012
* Microsoft Windows 2012 R2

#### Chef
- Chef 11+

#### Cookbooks
* windows

Attributes
----------

There are individual attributes within the attributes files for the URL, checksum and package name of each Visual C++ runtime major and minor version.

If you wish to install anything except the latest packages, you may set one of

* ```node['vcruntime']['vc9']['version']```
* ```node['vcruntime']['vc10']['version']```
* ```node['vcruntime']['vc12']['version']```

to the appropriate version.

Usage
-----

Just include `vcruntime::vc9`, `vcruntime::vc10`, or vcruntime::vc12 in your node's `run_list`:

```json
{
  "name": "my_node",
  "run_list": [
    "recipe[vcruntime::vc9]"
  ]
}
```

License and Authors
-------------------

**Author:** Yvo Van Doorn (<yvo@chef.io>)

**Author:** Dan Robinson (<drobinson@chef.io>)

**Author:** Julian Dunn (<jdunn@chef.io>)

**Copyright:** 2013-2015, Chef Software, Inc.
```
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

