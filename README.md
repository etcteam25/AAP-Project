# AAP-Project starter

Initial read-only Dell iDRAC discovery project for Ansible Automation Platform.

## Included

- `collections/requirements.yml`
- `playbooks/01_discover_idrac.yml`

## AAP setup

1. Import/push the files into your repository.
2. Sync the AAP Project.
3. Create a Job Template using `playbooks/01_discover_idrac.yml`.
4. Add a Survey text field:
   - Question: `iDRAC IP`
   - Variable: `idrac_ip`
   - Required: Yes
5. Attach an AAP credential that injects:
   - `IDRAC_USERNAME`
   - `IDRAC_PASSWORD`
6. Run the Job Template.

This first playbook is read-only. It does not create RAID, reboot the server,
change boot order, or erase disks.
