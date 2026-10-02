# GitHub Profile Setup

## What this folder contains

```text
dekuotaku123/
├── README.md
└── .github/
    └── workflows/
        └── snake.yml
```

You do NOT need Node.js, Python, npm, or any other software for this setup.

## Step 1 — Open your profile repository

Open:

https://github.com/dekuotaku123/dekuotaku123

This is the special repository whose README appears on your GitHub profile.

## Step 2 — Replace README.md

Open the repository and replace the existing `README.md` with the `README.md`
from this folder.

Commit the change to the `main` branch.

## Step 3 — Add the workflow

Inside the same repository create:

```text
.github/workflows/snake.yml
```

Paste the supplied `snake.yml` into that file and commit it.

## Step 4 — Give GitHub Actions write permission

In the repository:

Settings
→ Actions
→ General
→ Workflow permissions
→ Read and write permissions
→ Save

This lets the workflow publish the generated snake SVG to the `output` branch.

## Step 5 — Run the animation once

Open:

Actions
→ Generate Snake Animation
→ Run workflow

Select the `main` branch if GitHub asks.
Then click **Run workflow**.

Wait for the workflow to finish successfully.

## Step 6 — Refresh your profile

Open:

https://github.com/dekuotaku123

Refresh the page.

The README, animated typing banner, stats, contribution graph and snake
animation should appear.

## If the snake is missing

Open the repository and check whether an `output` branch was created.

If the workflow failed:
1. Open Actions.
2. Open the failed "Generate Snake Animation" run.
3. Open the failed step.
4. Read the error shown by GitHub.

## Recommended final repository layout

```text
dekuotaku123
│
├── README.md
│
└── .github
    └── workflows
        └── snake.yml
```

Nothing else is required.

## Important

Do not rename the profile repository. It must remain:

```text
dekuotaku123/dekuotaku123
```
