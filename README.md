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

    - hosts: servers
      roles:
          - itrunsde.logscale
            vars:
              - installer: "humio-log-collector_1.5.2_linux_amd64.deb"
              - token: "xxxxxxxxxx"

License
-------

MIT

Author Information
------------------

Further information on the author or their work can be found at [https://mylogscale.com](https://mylogscale.com).
