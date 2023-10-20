Install and enroll Falcon LogScale Collector agent
=========

Installation and enrolment of the Falcon LogScale Collector agent on Linux distributions. 

Requirements
------------

Provision of the installation file from the Falcon LogScale Download Portal.

Role Variables
--------------

- `installer_file` for installing the collector agent on the system
- `enrollment_token` is needed for the enrollment to the LogScale platform


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
---
- hosts: servers
  roles:
    - name: itrunsde.logscale
      vars:
      - installer: "humio-log-collector_1.5.3_linux_amd64.deb"
      - enrollment_token: "xxxxxxxxxx"
```

License
-------

MIT

Author Information
------------------

Further information on the author or their work can be found at [https://mylogscale.com](https://mylogscale.com).
