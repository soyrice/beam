<!--
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->
{% for sdk_version in py-deps-data.sdk_versions %}
<details><summary markdown="span"><b>{{ sdk_version.sdk_version_number }}</b></summary>

<p>Beam SDK for Python {{ sdk_version.sdk_version_number }} has the following compile and runtime dependencies.</p>

<table class="table-bordered table-striped">
<tr><th>Package</th><th>Version</th></tr>
  {% for dependency in sdk_version.dependencies %}
  <tr><td>{{ dependency.package_name }}</td><td>{{ dependency.package_version }}</td></tr>
</table>
</details>