# Git and GitHub basics

Welcome. This is the starter project — the one that teaches the loop every other project
here uses. **Nothing to install except git.**

## Check you have git

```bash
git --version
```

If that prints a version, you are ready.

## Tell git who you are, once

```bash
git config --global user.name "Your Name"
git config --global user.email "the-email-you-use-for-github@example.com"
```

Use the same email as your GitHub account, or your commits will not be linked to you.

## Where the work is

Open the **Issues** tab above. There are four, in order. **Every command you need is written
inside the ticket** — you are not expected to remember them or look them up.

The loop you will run four times:

```bash
git checkout main
git pull                       # catch up before branching
git checkout -b my-branch
# ...make your change...
git add <the file>
git commit -m "Say what changed"
git push -u origin my-branch
```

Then open a **Pull Request** on GitHub and write `Closes #1` in the description, with the
issue number you are working on.

## What happens next

Raj reviews every pull request. On **ticket 2 he will ask you to change something on
purpose** — so that the first time you meet a code review, it is on a one-line file that does
not matter.

When he asks for a change, push another commit to the **same branch**. Do not open a second
pull request — a pull request follows a branch, so your new commit appears in it and the
review runs again.

## The one rule

**Never commit directly to `main`.** If you do it by accident, say so in Slack. It is a
two-minute fix and a normal thing to get wrong once.

## Why this repository is nearly empty

Deliberately, and it is the one template in the library that is meant to stay this way.

Every other project here starts you from a scaffold — the boring setup done, so you can get to
the actual work. This one cannot, because **creating your first file, committing it and opening
a pull request IS the work.** A repository that arrived with files already in it would have done
the exercise for you.

(If you are an engineer auditing the templates: this is not the thin-template gap that DZ-382
fixed elsewhere. It is a decision, recorded here so it does not get "fixed".)
