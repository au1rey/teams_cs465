# Activity: Git with the Flow [^1]

Practice setting up and running a team project using Git-Flow on GitHub.

## Overview

![greengoblinmascot](media/gg.jpeg)

Each member of the team is chair of a different department at Green State University (_"Go Goblins!"_). Each chair's job is to produce a course listing for the upcoming Summer session.  The usual courses aren't offered then, so you must come up with some new courses your department will offer.

Each course listing must have:

- 4 character department code (e.g., MATH or ENGL) & course number (000-999)
- title (up to 30 chars)
- description (up to 80 chars)

The courses should be listed by department in course # order in the [`catalog.md`](./catalog.md) file. Each word of the course title should be capitalized, except for words with fewer than 4 characters. The description should be formatted as normal English sentences.

The courses are listed in the associated department files (e.g., `math.md`) which are hyperlink'ed from the `catalog.md` file.

For example, in the English department you might offer:

---
**ENGL007** _Poetry of Ian Fleming_
> Study of verse from the spy master.

**ENGL042** _Don't Panic Yet!_
> Societal commentaries of Douglas Adams.

---

Using Markdown, you can produce this layout using the following:

```text
---

**ENGL007** _Poetry of Ian Fleming_
> Study of verse from the spy master.

**ENGL042** _Don't Panic Yet!_
> Social commentaries of Douglas Adams. 

---
```

Humor is encouraged, but keep it PG-13.

When finished, the `main` branch of your repository will contain a complete markdown version of the Summer session catalog.

You are provided a primary markdown file, [`catalog.md`](./catalog.md), to which you will add or update links to each of the departments' markdown files.

> This is the only activity where we **don't** want you to talk **directly** to other members of your team.  Instead, use Teams for all communications between members of the team, like a modern programming team of at office, at home, or geographically distributed team.  

## Steps

1. **One** team member is chosen as the "Project Lead" who then accepts the [activity assignment](https://classroom.github.com/a/oM0TW613) from GitHub Classroom as usual.  

    a. clone the activity repository using the link on BrightSpace
    b. make sure the new repo is private.  
    c. set GitHub to [protect the main branch](https://learn.snhu.edu/d2l/le/content/2366228/viewContent/54950648/View).  
    d. invite other team members to join the repo, each having the  `maintain` role:  

    ```  
    Settings -> Collaborators and teams->...  
    ```

2. Team decides which member will handle which department. If you don't have enough people to handle the five subjects, either double-up or just omit subjects (if omitting one be sure to update `catalog.md`). 

3. Each team member does the following:
  - Accept the invitation from the Project Leader and clone the repository.
  - `cd` into the cloned repo.
  - Create a local feature branch for your work, with a name indicating the department you are handling, e.g., `math-department`.  
  - Switch to that new feature branch.
  - Add at least 4 classes to the corresponding `.md` file (e.g., `math.md`).
  - Edit the `catalog.md` file to add your username in the department chair slot of the department you selected.
  - Push your branch to GitHub.

  	`git push -u origin branch-name`
  - Preview your branch on GitHub. Is content correct? Does the formatting meet the requirements? Are any words spelled incorrectly?
  - If everything is correct, open a Pull Request for your branch.  

4. Respond to Pull Requests (everyone).
    - When you see a Pull Request from a team member, review their
        branch on GitHub.
    - Comment on their Pull Request.
        - Formatting or spelling problems? Are prices consistent?
        - Items in alphabetical order?
        - Do you approve the merge into main?  If so, then do it.

5. Merge & Close Pull Request (feature author).
    - Respond to comments to your Pull Request. If problems, fix them
        & push again.
    - After your team _approves your work_, merge your branch into `main`.
    - If GitHub cannot do an automatic merge, it probably means that `main` has changed since you cloned it. In that case do the following:
        1. `git fetch` main from GitHub to your local repo and merge into your local `main`.
        2. Merge your feature branch into main on your machine. Fix any conflicts, and if you repair any conflicts you need to commit again afterwards.
        3. Push your (merged) main to GitHub. This time it should succeed. If you made any changes to your feature branch, push those, too.



## FINAL STEP

The project lead:
1. ensures that the team repository is fully up to date on GitHub, then
2. the project lead invites the instructor (GitHub username `ccpalmer`) to join the repository.

<div style="color:green;font-size:20;text-align:center;"><i>Go Green Goblins!</i></div>

---

[^1]: _Based on the excellent example assignment at `https://github.com/ISP21/ku-cafe`._
