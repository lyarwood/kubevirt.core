=============================================
KubeVirt Collection for Ansible Release Notes
=============================================

.. contents:: Topics

This changelog describes changes after version 1.0.0.

v1.5.0
======

Release Summary
---------------

Support for stopped VMs, deprecation of the 'connections' parameter and many cleanups.

Major Changes
-------------

- chore: Update supported ansible-core versions to >=2.15 `#105 <https://github.com/kubevirt/kubevirt.core/pull/105>`_
- feat,test(inventory): Support listing stopped VMs and major rework of unit tests  `#114 <https://github.com/kubevirt/kubevirt.core/pull/114>`_

Minor Changes
-------------

- Bump e2e software versions `#109 <https://github.com/kubevirt/kubevirt.core/pull/109>`_
- Make kubevirt_vm tests more robust `#103 <https://github.com/kubevirt/kubevirt.core/pull/103>`_
- Several minor improvements `#115 <https://github.com/kubevirt/kubevirt.core/pull/115>`_
- chore: Ensure compatibility with kubernetes.core >=3.1.0,<6.0.0 `#111 <https://github.com/kubevirt/kubevirt.core/pull/111>`_
- kubevirt_vm integration tests: changed ssh key type to RSA for FIPS mode `#108 <https://github.com/kubevirt/kubevirt.core/pull/108>`_

Bugfixes
--------

- fix(tests,kubevirt_vm): Fix assertion in verify.yml `#106 <https://github.com/kubevirt/kubevirt.core/pull/106>`_

v1.4.0
======

Release Summary
---------------

Compatibility with kubernetes.core >=3.1.0,<4.1.0 and some minor enhancements.

Minor Changes
-------------

- Provide links for docsite and improve docs by adding markup `#95 <https://github.com/kubevirt/kubevirt.core/pull/95>`_
- cleanup: Cleanup YAML passed to k8s module `#88 <https://github.com/kubevirt/kubevirt.core/pull/88>`_
- docs: Use proper type for connections parameter `#90 <https://github.com/kubevirt/kubevirt.core/pull/90>`_
- feat(kubevirt_vm_info): Set wait_condition based on running `#91 <https://github.com/kubevirt/kubevirt.core/pull/91>`_

Bugfixes
--------

- fix(kubevirt_vm): Set wait_condition based on running `#89 <https://github.com/kubevirt/kubevirt.core/pull/89>`_
- fix: Ensure compatibility with kubernetes.core >=3.10,<4.1.0 `#100 <https://github.com/kubevirt/kubevirt.core/pull/100>`_

v1.3.2
======

Release Summary
---------------

No functional changes, hotfix release to retrigger the downstream build and to keep in sync with Ansible Automation Hub.

v1.3.1
======

Release Summary
---------------

No functional changes, only updates to the shipped documentation.

v1.3.0
======

Minor Changes
-------------

- feat: Add append_base_domain option to connections `#72 <https://github.com/kubevirt/kubevirt.core/pull/72>`_
- feat: Give secondary interfaces a higher priority over services `#76 <https://github.com/kubevirt/kubevirt.core/pull/76>`_

Bugfixes
--------

- feat: Set ansible_connection to winrm for Windows hosts `#75 <https://github.com/kubevirt/kubevirt.core/pull/75>`_
- fix: Explicity set ansible_port `#70 <https://github.com/kubevirt/kubevirt.core/pull/70>`_
- fix: Return early to avoid adding empty groups. `#73 <https://github.com/kubevirt/kubevirt.core/pull/73>`_

v1.2.3
======

Release Summary
---------------

No functional changes, hotfix release to retrigger the downstream build and to keep in sync with Ansible Automation Hub.

v1.2.2
======

Release Summary
---------------

No functional changes, only cleanup of files included in the release tarball and vendoring of documentation fragments.

v1.2.1
======

Release Summary
---------------

Mostly code cleanups and dependency updates to ensure compatibility with KubeVirt >= 1.1.0

v1.2.0
======

Release Summary
---------------

Not released due to issues in the release process

v1.1.0
======

Minor Changes
-------------

- Add kubevirt_vm_info module to describe existing VirtualMachines
- inventory: Allow to control creation of additional groups
- inventory: Drop creation of the namespace_vmis_group as it is redundant

v1.0.0
======

Release Summary
---------------

Initial release
