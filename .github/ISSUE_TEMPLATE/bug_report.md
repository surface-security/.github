name: "\U0001F41B Bug report"
description: "When something isn't working as expected or documented"
labels: ["bug", "needs-triage"]
body:
- type: markdown
  attributes:
    value: |
      Thank you for opening an issue. Please note that we try to keep the 
      <project> issue tracker reserved for bug reports and feature requests. 
- type: checkboxes
  attributes:
    label: Confirmation
    description: Please make sure to have followed the following checks.
    options:
      - label: My issue isn't already found on the issue tracker.
        required: true
      - label: I have replicated my issue using the latest version of the provider and it is still present.
        required: true
- type: textarea
  attributes:
    label: Related software versions.
    description: |
      Validate the software version of the related components by checking the containers running, the services you are 
      connected to and/or simply by checking your local `docker-compose` files.
  validations:
    required: true
- type: textarea
  attributes:
    label: Affected resource(s)
    description: |
      Please list the resources as a list, for example:
      - x
      - y
      - z

      If this issue appears to affect multiple resources, please mention this.
  validations:
    required: true
- type: input
  attributes:
    label: Link to debug output
    description: |
      A link to the output (https://gist.github.com) provided.  **Do not truncate or trim the output as the 
      surrounding context is useful for debugging and without it, maintainers are restricted in what assistance 
      and diagnosis they can provide**. 
      
      Be sure to redact or sanitise any sensitive information (such as API keys or tokens) in 
      your logs.
  validations:
    required: true
- type: textarea
  attributes:
    label: Panic output
    description: Output from a crash or panic.
  validations:
    required: false
- type: textarea
  attributes:
    label: Expected output
    description: What did you expect to happen?
  validations:
    required: true
- type: textarea
  attributes:
    label: Actual output
    description: What actually happened?
  validations:
    required: true
- type: textarea
  attributes:
    label: Steps to reproduce
    description: How can your issue be replicated?
    placeholder: |
      1. ...
      2. ...
      3. ...
  validations:
    required: true
- type: textarea
  attributes:
    label: Additional factoids
    description: Is there any other important information you'd like to share?
  validations:
    required: false
- type: textarea
  attributes:
    label: References
    description: Are there any other GitHub issues (open or closed) or Pull Requests that should be linked here? 
  validations:
    required: false
