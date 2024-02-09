name: "Documentation"
description: "Improvements or additions to documentation"
title: "[DOC] "
labels: ["documentation"]
body:
 
  - type: textarea
    id: what-needs-to-be-done
    attributes:
      label: "Was muss dokumentiert werden?"
    validations:
      required: true

  - type: textarea
    id: how-should-it-be-done
    attributes:
      label: "Wie sollte es dokumentiert werden?"
    validations:
      required: false
 
  - type: dropdown
    id: version
    attributes:
      label: "Priorität:"
      description: Wie wichtig ist das Refactoring?
      options:
        - Wäre eine nette, lokale Verbesserung
        - Hat größere Auswirkungen auf die Codequalität
        - Hat große Auswirkungen auf die Struktur
      default: 1
    validations:
      required: true

  - type: dropdown
    id: version
    attributes:
      label: "Sichtbarkeit:"
      description: Für wen ist diese Dokumentation?
      options:
        - Nur Entwickler
        - Entwickler und Product Owner
        - Partner / Kunde
      default: 0
    validations:
      required: true
 
  - type: textarea
    id: comment
    attributes:
      label: "Kommentar"
    validations:
      required: false
 
