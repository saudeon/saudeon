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
  nationality: "🇦🇺",
  location: "Los Angeles",
  position: .staff,
  openToWork: false
)
```

<!--
**saudeon/saudeon** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
