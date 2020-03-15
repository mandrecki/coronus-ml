## Setup

1. Install Python 3.8

2. Clone this and coronous repo
```
git clone git@github.com:mandrecki/coronus-ml.git
git clone git@github.com:mandrecki/coronus.git
```

3. Setup your Python environment and install this package
```
cd coronus-ml
virtualenv --python=/usr/bin/python3.8 venv
source venv/bin/activate
pip install ../coronus
pip install -e .
```
4. Configure git (you can add `--global` if you would like to set this for your
entire systems, not just this repo):
```
git config user.name "Your Name"
git config user.email "your@email"
git config pull.rebase true 
git config branch.autosetuprebase always
```

## Devel process

(needs polishing...)

Create your branch

```
git branch yourbranch
git checkout yourbranch
```

Make some changes and commit

```
git add new_file.txt
git commit -m "meaningful changes..."
```

Submit a pull request. You want to merge into *staging* (so your code can be used to generate new data and tested with the app), but first others should review your code. Describe the changes briefly and tag relevant coders as reviewers.
