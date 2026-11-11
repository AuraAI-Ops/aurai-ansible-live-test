# aurai-ansible-live-test

Ansible playbook for the AuraAI live test on dev (dev.auraai.ai).

- `junos/show_version.yml` runs `show version` on a Juniper device over netconf. It is read-only: it changes nothing on the device.
- This repo holds only this one playbook on purpose. The orch safety check reads every playbook in a project, so a project must not contain unrelated playbooks.
- Public because the run fetches it without git credentials. Keep it free of secrets.
