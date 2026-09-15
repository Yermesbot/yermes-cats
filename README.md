# yermes-cats

Mood cats used by [Yermes](https://github.com/apps/Yermesbot) to signal reviewer mood
at the top of a PR review.

Each image is a single panel cropped from a 4x5 labeled mood grid. Filenames are
`NN-slug.jpg` where the slug is the mood name used by the review scripts.

Referenced from review bodies via:

    https://raw.githubusercontent.com/Yermesbot/yermes-cats/main/cats/NN-slug.jpg

Public by design: GitHub's image proxy (camo) cannot fetch private raw URLs, so the
cats must be hosted in a public repo to render inside reviews on private repos.
