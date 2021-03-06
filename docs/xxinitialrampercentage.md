<!--
* Copyright (c) 2017, 2018 IBM Corp. and others
*
* This program and the accompanying materials are made
* available under the terms of the Eclipse Public License 2.0
* which accompanies this distribution and is available at
* https://www.eclipse.org/legal/epl-2.0/ or the Apache
* License, Version 2.0 which accompanies this distribution and
* is available at https://www.apache.org/licenses/LICENSE-2.0.
*
* This Source Code may also be made available under the
* following Secondary Licenses when the conditions for such
* availability set forth in the Eclipse Public License, v. 2.0
* are satisfied: GNU General Public License, version 2 with
* the GNU Classpath Exception [1] and GNU General Public
* License, version 2 with the OpenJDK Assembly Exception [2].
*
* [1] https://www.gnu.org/software/classpath/license.html
* [2] http://openjdk.java.net/legal/assembly-exception.html
*
* SPDX-License-Identifier: EPL-2.0 OR Apache-2.0 OR GPL-2.0 WITH
* Classpath-exception-2.0 OR LicenseRef-GPL-2.0 WITH Assembly-exception
-->

# -XX:InitialRAMPercentage

This Oracle Hotspot option can be used to specify the initial size of the Java heap as a percentage of the total memory available to the VM. The option is recognized by the OpenJ9 VM and is provided for compatibility.

## Syntax

        -XX:InitialRAMPercentage=N

: Where N is a value between 0 and 100, which can by of type "double". For example, 12.3456.

<i class="fa fa-pencil-square-o" aria-hidden="true"></i> **Note:** If you set a value for [`-Xms`](xms.md), this option is ignored.

If your application is running in a container and you have specified [`-XX:+UseContainerSupport`](xxusecontainersupport), both the default heap size for containers and the `-XX:InitialRAMPercentage` option are based on the available container memory.


<!-- ==== END OF TOPIC ==== xxinitialrampercentage.md ==== -->
