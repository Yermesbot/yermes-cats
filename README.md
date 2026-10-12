# yermes-cats

Mood cats used by [Yermes](https://github.com/apps/Yermesbot) to signal reviewer mood
at the top of a PR review.

Filenames are `NN-slug.jpg` where the slug is the mood name used by the review
scripts. Panel numbers are append-only: they are baked into every posted review.

- `01`-`20`: cats, each a single panel cropped from a 4x5 labeled mood grid.
- `21`-`26`: trail-cam wildlife, each tied to a review situation:

| # | animal | slug | situation |
|---|--------|------|-----------|
| 21 | jaguar | `wait-whats-this` | found something odd in the diff |
| 22 | polar bear cub | `nose-deep-nitpicking` | line-by-line read, lots of small things |
| 23 | tiger | `intense-scrutiny` | hard look at every line |
| 24 | cougar | `deeply-unimpressed` | Request Changes before writing a comment |
| 25 | elk | `lgtm-whatever` | cheeky rubber-stamp approval |
| 26 | snow leopards | `looping-in-backup` | concerning; another human should look |

Referenced from review bodies via:

    https://raw.githubusercontent.com/Yermesbot/yermes-cats/main/cats/NN-slug.jpg

Public by design: GitHub's image proxy (camo) cannot fetch private raw URLs, so the
cats must be hosted in a public repo to render inside reviews on private repos.
