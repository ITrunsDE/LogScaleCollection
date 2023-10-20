Enroll Falcon LogScale Collector agent
=========

Enrolment of the Falcon LogScale Collector agent on Linux distributions. 

Requirements
------------

Installed Falcon LogScale Collector on the system. 

Role Variables
--------------

- `enrollment_token` is needed for the enrollment to the LogScale platform


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
---
- hosts: servers
  roles:
    - name: itrunsde.logscale_collector.enroll
      vars:
        - enrollment_token: "xxxxxxxxxx"
```

License
-------

MIT

Author Information
------------------

Further information on the author or their work can be found at [https://mylogscale.com](https://mylogscale.com).
