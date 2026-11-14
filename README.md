# Trawl Home Assistant add-on

Wraps the upstream [trawl](https://github.com/germondai/trawl) image (`ghcr.io/germondai/trawl`).
Nothing is built: Supervisor pulls the tag named by `version` in `trawl/config.yaml`.

A daily GitHub Action bumps `version` to the newest upstream release once it is
at least 3 days old and its image tag exists on ghcr.io. Enable **Auto update** in HA to follow it.

Install: Settings → Add-ons → Add-on Store → ⋮ → Repositories → add this repo's URL.
