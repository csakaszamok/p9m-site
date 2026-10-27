# p9m.dev

The homepage of [Purgatorium (p9m)](https://github.com/csakaszamok/p9m): plain HTML in `html/`, served by nginx.

## How it is deployed

It runs in a Purgatorium sandbox that never sleeps. [doco-cd](https://github.com/kimdre/doco-cd) in that sandbox
polls this repository and runs `docker compose up --build` on every push to `main`, so a merged change is live within
a minute or two.

## Trying it locally

```sh
docker compose up --build
```

Then open <http://localhost:8080>.
