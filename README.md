```swift
import Foundation

enum Position: String {
  case senior, staff
}

struct Project {
  let name: String
  let url: String
}

struct Engineer {
  let name: String
  let nationality: String
  let location: String
  let position: Position
  let projects: [Project]?
  let openToWork: Bool

  init(_ name: String,
       nationality: String,
       location: String,
       position: Position,
       projects: [Project]? = nil,
       openToWork: Bool) {
    self.name = name
    self.position = position
    self.location = location
    self.nationality = nationality
    self.projects = projects
    self.openToWork = openToWork
  }

}

let me = Engineer(
  "Sebastien Audeon",
  nationality: "š¦šŗ",
  location: "Los Angeles",
  position: .staff,
  openToWork: false
)
```

<!--
**saudeon/saudeon** is a āØ _special_ āØ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- š­ Iām currently working on ...
- š± Iām currently learning ...
- šÆ Iām looking to collaborate on ...
- š¤ Iām looking for help with ...
- š¬ Ask me about ...
- š« How to reach me: ...
- š Pronouns: ...
- ā” Fun fact: ...
-->
