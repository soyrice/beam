---
layout: section
title: "Python SDK dependencies"
section_menu: section-menu/sdks.html
permalink: /documentation/sdks/python-dependencies/
---
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

# Beam SDK for Python dependencies

The Beam SDKs depend on common third-party components which then
import additional dependencies. Version collisions can result in unexpected
behavior in the service. If you are using any of these packages in your code, be
aware that some libraries are not forward-compatible and you may need to pin to
the listed versions that will be in scope during execution.

<p>To see the compile and runtime dependencies for your Beam SDK version, expand
the relevant section below.</p>

{{% assign py-deps-data=site.data.python-sdk-dependencies %}}

{{% include python-sdk-dependencies.md %}}
