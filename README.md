# Travel

Commits from around the world. Open [travel.geojson](travel.geojson) to see the places

## Goal

Save the location of the places I've visited/stayed.

## How it works

This repo uses a `pre-commit` hook that retrieves the location using OSX's Core Location API through [WhereAmI](https://github.com/victor/whereami). Then it writes it to `travel.geojson`.

## How to use it

1. Fork the repo
1. Install WhereAmI (`brew tap victor/whereami && brew install whereami`)
1. Copy `pre-commit` hook to your `.git` folder (`copy pre-commit
   .git/hooks`)
1. Remove `travel.geojson` and do a commit without hooks (`git commit -m
   'start over' -n`)
1. Start doing commits (ex. `git commit -m "Stockholm" --allow-empty`)

## License

Check [LICENSE](LICENSE)
