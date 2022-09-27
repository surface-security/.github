name: "\U0001F680 Feature request"
description: "Suggest a new feature or other enhancement"
labels: ["enhancement", "needs-triage"]
body:
- type: markdown
  attributes:
    value: |
      Thank you for opening an issue. Please note that we try to keep the 
      <project> issue tracker reserved for bug reports and feature requests. 
- type: textarea
  attributes:
    label: Related software versions 
    description: |
      Validate the software version of the related components by checking the containers running, the services you are 
      connected to and/or simply by checking your local `docker-compose` files.
  validations:
    required: true
- type: textarea
  attributes:
    label: Description
    description: Provide a quick (or expanded!) overview of the proposed change.
  validations:
    required: true
- type: textarea
  attributes:
    label: Use cases
    description: |
      In order to properly evaluate a feature request, it is necessary to understand
      the use-cases for it. Please describe below the _end goal_ you are trying 
      to achieve that has led you to request this feature.

      Please keep this section focused on the problem and not on the suggested
      solution. We'll get to that in a moment, below!
  validations:
    required: true
- type: textarea
  attributes:
    label: References
    description: |
      Are there any other GitHub issues, whether open or closed, that are related to
      the problem you've described above or to the suggested solution? If so, please
      create a list below that mentions each of them. 
  validations:
    required: false

