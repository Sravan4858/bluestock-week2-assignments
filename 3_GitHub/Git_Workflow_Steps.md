# Git and GitHub: steps to create the repo with version history

## One-time setup
```bash
git config --global user.name "M. Sravam"
git config --global user.email "mannesravan82@gmail.com"
```

## 1. Create the repo on GitHub
github.com > New repository > name `bluestock-week2-assignments` > Public > add a README > Create.

## 2. Clone it
```bash
git clone https://github.com/<your-username>/bluestock-week2-assignments.git
cd bluestock-week2-assignments
```

## 3. Add each assignment as a separate commit
Copy the `1_Stock_Market`, `2_API_Assignment`, `4_Architecture_Diagram` and `5_FinTech_Research` folders in one at a time:
```bash
git add 1_Stock_Market
git commit -m "Add stock market summary and Infosys financial analysis"
git add 2_API_Assignment
git commit -m "Add API extraction script, docs and CSV output"
git add 4_Architecture_Diagram
git commit -m "Add data flow architecture diagram"
git add 5_FinTech_Research
git commit -m "Add Zerodha FinTech research report"
git push origin main
```

## 4. Branch and pull request (shows you know the workflow)
```bash
git checkout -b update-readme
# edit README.md
git add README.md
git commit -m "Update README with project overview"
git push -u origin update-readme
```
On GitHub, click "Compare and pull request", then "Create pull request", then "Merge pull request".
```bash
git checkout main
git pull origin main
```

## 5. Evidence
Open the repo > Commits, take a screenshot, and save it as `commit_history.png`.

## Quick reference
| Command | Purpose |
|---|---|
| `git clone` | Copy a remote repo to your computer |
| `git add` | Stage changes |
| `git commit` | Save a snapshot with a message |
| `git push` | Upload commits to GitHub |
| `git pull` | Download and merge new commits |
| `git checkout -b` | Create and switch to a new branch |
