---
name: Bug report
about: Found an issue? Create an issue... and send it to McDonald's
title: "[BUG]"
labels: bug
assignees: ''
body:
- type: textarea
  id: description
  attributes:
    label: Describe the bug
    description: A clear and concise description of what the bug is.
    render: bash
  validations:
    required: true
- type: textarea
  id: repro
  attributes:
    label: Reproduction steps
    description: "How do you trigger this bug? Please walk us through it step by step."
    value: |
      1.
      2.
      3.
      ...
    render: bash
  validations:
    required: true
- type: textarea
  id: behavior_expected
  attributes:
    label: Expected behavior
    description: What should have happened?
    render: bash
  validations:
    required: true
- type: textarea
  id: behavior_actual
  attributes:
    label: Actual behavior
    description: What should actually happened?
    render: bash
  validations:
    required: true
- type: input
  id: platform
  attributes:
    label: What platform were you on?
    placeholder: Android 16
  validations:
    required: true
- type: dropdown
  id: which-app
  attributes:
    label: Which app has this issue? 
    options:
      - USA
      - Global
      - Japan
      - Guatemala
      - Honduras
      - Nicaragua
      - Israel
      - Other
  validations:
    required: true
- type: input
  id: app-version
  attributes:
    label: App Version
    description: Check your OS's app information for this
    placeholder: 25.71.2
  validations:
    required: true
- type: checkboxes
  id: acknowledge
  attributes:
    label: Please acknowledge any that apply
    description: You may select more than one.
    options:
      - label: I will [send](https://www.mcdonalds.com/us/en-us/feedback.html) this bug report to McDonald's.
        required: true
      - label: This repository is not affiliated with McDonald's Corperation.
        required: true
---

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Additional context**
Add any other context about the problem here.
