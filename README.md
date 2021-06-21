# Run playbook on Ansible Tower/AWX

Github action that allows you to run a playbook on Ansible Tower/AWX.

This project was cloned/adopted from https://github.com/vortegon/github-action-ansible-tower, cleaned-up, and updated dependencies. Thank you for the original contribution.

## Usage

```yaml
uses: certara/github-action-ansible-tower@v1.0.0
with:
  ansible-tower-user: ${{ secrets.ansibleUser }}
  ansible-tower-pass: ${{ secrets.ansiblePass }}
  ansible-tower-url: ${{ secrets.ansibleUrl }}
  template-id: "1254"
  additional-vars: |
  {
      "example_aws_environment": "dev",
      "example_1": "someother_value",
      "example_2": "someother_value"
  }
```
