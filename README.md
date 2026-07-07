[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/AjDMoFtn)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=24216991)
# Mini-Project - Build Your Own Game!

## For Students

### The Project
Design and build your own game in Python. It can be a terminal game (typed answers) or a turtle game (keys and mouse clicks). There are only two requirements:

1. **Your game must use user input** — mouse clicks, key strokes, typed answers, etc.
2. **Your game must keep track of and display a score.**

Everything you've learned in Modules 1-6 is fair game: variables, `input()`, `if`/`elif`/`else`, `while` loops, `for` loops, lists, `random`, and turtle graphics. Open `mini_project.py` for game ideas, helpful code snippets, and optional level-up ideas.

### Getting Started
1. Accept the assignment invite link provided by your instructor
2. Once your repo is created, click the green **Code** button and select **Open with Codespaces**
3. Open `mini_project.py` and start building

### Playing a Turtle Game in Codespaces
1. Run your game: `python mini_project.py`
2. Open the **PORTS** tab, click the globe icon on port **6080** ("Turtle Desktop")
3. Click **Connect**, password: **`vscode`**
4. Click inside the turtle window once so it hears your keyboard!

### Submitting
- Commit and push like always: **Source Control** icon, type a message, **Commit**, then **Sync Changes**
- The autograder checks that the two requirements are present in your code. **Whether your game works and is fun is graded by your instructor playing it** — so playtest it yourself first!
- You can push as many times as you like before the deadline

---

## For Instructors

### How This Repo Works
- `mini_project.py` — the student-facing template: the two requirements, game ideas for both terminal and turtle paths, code snippets, and optional stretch ideas
- `tests/test_mini_project.py` — autograder; see the note below
- `.github/workflows/grade.yml` — GitHub Action that runs on every push to `main` and posts results as a commit comment
- `.devcontainer/devcontainer.json` — Codespaces environment (Python 3.11, desktop-lite VNC on port 6080 for turtle games, AI features disabled)

### A Note on Grading an Open-Ended Game
A student game may block on input(), loop forever, or open a turtle window, so the
autograder **never runs it**. Like Module 5, it parses `mini_project.py` with `ast` and
verifies the requirements exist in the code: an input mechanism (`input()`, or turtle's
`onkey`/`onclick`/`listen`), a score variable (name containing "score" or "point"), code
that changes the score, code that displays it (`print`/`write`/`title` with the score
variable), and at least some game logic (`if`/`while`/`for`). This is a requirements
check only — **play each game** for the real grade. Have students demo on the projector;
it's the best part of the week.

### Setting Up GitHub Classroom
1. Go to [classroom.github.com](https://classroom.github.com) and create/open your classroom
2. Click **New assignment** and use this repo as the starter code
3. Set visibility to **Private**
4. Add an autograding test (**Run command**: `python tests/test_mini_project.py`) for the requirements check; combine with your play-test grade
5. Consider protecting `tests/` and `.github/` via **protected file paths**
6. Share the generated invite link with students
