name: Grant access to github/<repo>
description: Fill this out if you need to gain access to a repo in the GitHub org
title: "Granting access to github/<repo> for @<handle>"
labels: ["Waiting for Manager Review", "github"]

body:
- type: checkboxes
  id: confirm
  attributes:
    label: This is a last resort
    description: Security will only make repository access changes as a last resort. I confirm that I have attempted to reach out to existing administrators of the repository and they have either left the business or are otherwise unable to make the required changes (e.g. on leave)
    options:
      - label: Yes
        required: true
      
  - type: textarea
    id: reason
    validations:
      required: true
    attributes:
      label: Describe why the change is required.

  - type: textarea
    id: account
    validations:
      required: true
    attributes:
      label: List the requested account(s)
      value: |
        - account1
        - account2
        - account3

  - type: dropdown
    id: roles
    validations:
      required: true
    attributes:
      label: Requested role
      multiple: false
      description: "Reference: https://github.com/github/github/settings/role_details"
      options:
        - Read
        - Triage
        - Write
        - Maintain
        - Admin
        - Limited write

  - type: textarea
    id: approval
    attributes:
      label: Who will approve this access?
      description: |
        @-mention your manager to get their approval.
        Once the approval is given, please remove the `Waiting for Manager Review` label. Otherwise the ticket will not be acted upon.
      value: |
        @-manager

        *Manager: Please add a comment to this issue with the words "I approve" or equivalent, and remove the `Waiting for Manager Review` label.*

  - type: textarea
    id: extra
    attributes:
      label: Extra information
      value: |
        /cc <related work> <related team>

  - type: markdown
    attributes:
      value: |
        [documentation](../blob/master/docs/how_to_grant_access_to_github_github.md) (note: these docs are for github/github but the general practices apply to all github org repos)
