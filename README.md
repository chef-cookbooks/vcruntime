vcruntime Cookbook
====================

Installs Microsoft VC runtime on Windows Azure

Requirements
------------
#### packages
- windows

Supported Platforms
-------------------
Microsoft Windows 2008 R2
Microsoft Azure ACS, blob, xSQL

Attributes
----------

#### vcruntime::default
<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['vc9']['x86']['tools']['pkg']['windows']['url']</tt></td>
    <td>String</td>
    <td>VC9 x86 source</td>
    <td><tt>http://download.microsoft.com/download/d/d/9/dd9a82d0-52ef-40db-8dab-795376989c03/vcredist_x86.exe</tt></td>
  </tr>
  <tr>
    <td><tt>['vc10']['x86']['tools']['pkg']['windows']['url']</tt></td>
    <td>String</td>
    <td>VC10 x86 source</td>
    <td><tt>http://download.microsoft.com/download/5/B/C/5BC5DBB3-652D-4DCE-B14A-475AB85EEF6E/vcredist_x86.exe</tt></td>
  </tr>
  <tr>
    <td><tt>['vc9']['x64']['tools']['pkg']['windows']['url']</tt></td>
    <td>String</td>
    <td>VC9 x64 source</td>
    <td><tt>http://download.microsoft.com/download/2/d/6/2d61c766-107b-409d-8fba-c39e61ca08e8/vcredist_x64.exe</tt></td>
  </tr>
  <tr>
    <td><tt>['vc10']['x64']['tools']['pkg']['windows']['url']</tt></td>
    <td>String</td>
    <td>VC10 x64 source</td>
    <td><tt>http://download.microsoft.com/download/3/2/2/3224B87F-CFA0-4E70-BDA3-3DE650EFEBA5/vcredist_x64.exe</tt></td>
  </tr>
</table>

Usage
-----
#### vcruntime::vc9 or vcruntime::vc10

Just include `vcruntime::vc9` or `vcruntime::vc10` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[vcruntime::vc9]"
  ]
}
```

License and Authors
-------------------
Author:: Yvo Van Doorn () Author:: Dan Robinson ()

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
