name: "Tests"
description: "Adding some form of quality control"
title: "[TEST] "
labels: ["tests"]
body:
 
  - type: textarea
    id: what-needs-to-be-done
    attributes:
      label: "Was muss getestet werden?"
      value: "- [ ] "
    validations:
      required: true
    
  - type: dropdown
    id: version
    attributes:
      label: "Priorität:"
      description: Wie wichtig sind diese Tests?
      options:
        - Optional / Nice to have
        - Standardtests einer Klassse
        - Coverage sonst nicht auf dev erfüllt
      default: 1
    validations:
      required: true
 
  - type: textarea
    id: comment
    attributes:
      label: "Kommentar"
    validations:
      required: false
 
