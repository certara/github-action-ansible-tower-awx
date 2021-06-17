# Run playbook on Ansible Tower

Github action that allows you to run a playbook on ansible tower.

## Usage

```yaml
uses: vortegon/github-action-ansible-tower@v1
with:
  ansible-tower-user: ${{ secrets.ansibleUser }}
  ansible-tower-pass: ${{ secrets.ansiblePass }}
  ansible-tower-url: ${{ secrets.ansibleUrl }}
  template-id: "1254"
  additional-vars: |
  {
      "var_environment": "dev",
      "var_1": "someother_value",
      "var_2": "someother_value"
  }
```
