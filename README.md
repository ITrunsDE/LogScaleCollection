# Ansible Collection - itrunsde.logscale_collector

The Falcon LogScale Collector Collection is used for easy installation and linking to the LogScale platform.

## Ansible version compatibility

Tested with the Ansible Core >= 2.13.0 versions, and the current development version of Ansible. Ansible Core versions before 2.13.0 are not supported.

## Included content

### Roles

| Role Name | Documentation | 
| --------- | :-----------: | 
| itrunsde.logscale_collector.install | [README](https://github.com/ITrunsDE/LogScaleCollection/blob/main/roles/install/README.md) | 

## Installing this collection

### Using `ansible-galaxy` CLI

To install the Falcon Ansible Collection using the command-line interface, execute the following:

```terminal
ansible-galaxy collection install itrunsde.logscale_collector
```

### Using a `requirements.yml` File

To include the collection in a `requirements.yml` file and install it through `ansible-galaxy`, use the following format:

```yaml
---
collections:
  - itrunsde.logscale_collector
```

Then run:

```terminal
ansible-galaxy collection install -r requirements.yml
```

### Additional notes

- **Upgrading the Collection**: Note that if you've installed the collection from Ansible Galaxy, it won't automatically update when you upgrade the `ansible` package. To manually upgrade to the latest version, use:

    ```terminal
    ansible-galaxy collection install itrunsde.logscale_collector --upgrade
    ```

- **Installing a Specific Version**: If you need to install a particular version of the collection (for example, to downgrade due to an issue), you can specify the version as follows:

    ```terminal
    ansible-galaxy collection install itrunsde.logscale_collector:==1.0.0
    ```

## Using this collection

### Example using modules

```yaml
---
- hosts: servers
  roles:
    - name: itrunsde.logscale
      vars:
      - installer: "humio-log-collector_1.5.2_linux_amd64.deb"
      - token: "xxxxxxxxxx"
```