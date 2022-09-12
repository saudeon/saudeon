```swift
import Foundation

enum Position {
  case junior, intermediate, senior, staff
}

struct Engineer {
  let name: String
  let position: Position
  let location: String
  let personalProjects: [Project]?
  
  init(_ name: String, 
       position: Position, 
       location: String, 
       projects: [Project]? = nil) {
    self.name = name
    self.position = position
    self.location = location
    self.personalProjects = projects
  }
  
}

struct Project {
  let name: String
  let url: String 
}

let me = Engineer(
  "Sebastien Audeon", 
  positon: .staff,
  location: "Los Angeles"
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
