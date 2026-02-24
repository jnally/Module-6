# Assignment Module 6 - Journal your learnings - Jeremy Nally

## Reflections on Chapter 13: Conflicts
I learned that executing a `git pull` is actually a two-step process in the background: first, it fetches the remote branch to a temporary location, and then it attempts to merge it into the local branch. If two different branches modify the exact same region of a file, Git will pause the merge and insert conflict markers (`<<<<<<< HEAD`, `=======`, `>>>>>>>`) directly into the code. I now know that resolving these conflicts requires manually opening the file, selecting the correct code to keep, deleting the markers, and finally staging and committing the resolved file.

## Reflections on Chapter 14: More About Conflicts
This chapter emphasized preventative measures. Before attempting any merge, it is incredibly useful to run `git diff branch1..branch2` to review the differences between the two branches. Moving forward, the best way to reduce conflicts is to rely entirely on Pull Requests rather than committing directly to main branches. As I continue to separate the React frontend code from the Python backend code for my math puzzle game, I will make sure each Pull Request strictly addresses one specific issue at a time to minimize overlapping file changes and keep the Git history clean.
