---
theme: ./
themeConfig:
  author: Max Mustermann
defaults:
  transition: slide-left
layout: intro
---

# Slidev Theme Starter

Presentation slides for developers

{{ $slidev.themeConfigs.author }}

---

# What is Slidev?

Slidev is a slide maker and presentation tool designed for developers. It includes the following features:

- 📝 **Text-based** - focus on your content with Markdown, then style it later
- 🎨 **Themable** - themes can be shared and reused as npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embed Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export to PDF, PPTX, PNGs, or even a hostable SPA
- 🛠 **Hackable** - virtually anything that's possible on a webpage is possible in Slidev

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)

---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel

## Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: section
---

# Some new section

## Some Subtitle

---
layout: quote
author: Max Mustermann (2025)
---

Some fancy quote

---
layout: cover
---

<word-cloud :list="[
'HTML',  
'Ember',  
'Sass',  
'FlexBox',  
'API',  
'VueJS',  
'Grid',  
'Rest',  
'JavaScript',  
'Animation',  
'React',  
'CSS',  
'Cache',  
'Less',  
'Svelte',  
'Angular',
'Spring Boot',
'Haskell',
'TDD',
'Monads',
'Applicatives',
'Mob Programming',
'Typescript'
]"/>

---

# Gantt

```mermaid
gantt
dateFormat MM-DD
axisFormat %m-%d
tickInterval 1week

section A
Analysis:active, a1, 03-09, 14d
Development: a2, after a1, 21d
```


---
layout: image-right-half
image: fh.jpg
---

# Code

Use code snippets and get the highlighting directly!

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

---
layout: end
author: Max Mustermann
student: 111111
email: max@example.com
---