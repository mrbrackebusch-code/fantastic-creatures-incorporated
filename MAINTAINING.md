# Maintaining Fantastic Creatures Incorporated

This repository is the durable source for one MakeCode Arcade tutorial specialized to **Dragon, Unicorn, and Phoenix**.

## Update process

- `README.md`, `pxt.json`, and `RELEASE_MANIFEST.json` are reproducible release outputs. Do not hand-edit them in the publication repository.
- The canonical learner copy, MakeCode templates, supplied world, generator, and validation sources live in the learning-game authoring repository.
- Regenerate and validate the fixed tutorial, then commit the updated release output to this same repository.
- Create releases through MakeCode's GitHub integration when the served tutorial must refresh from MakeCode's cloud cache.
- Keep the stable GitHub-backed MakeCode URL. Do not replace it with an anonymous or persistent MakeCode Share link.
- The tutorial URL must end with `/README` (without `.md`). Do not rely on implicit repository-root routing.
- Every construction beat has a native 320 × 240 gameplay GIF under `assets/demos`. Rebuild affected recordings after source/asset/behavior changes; retain the input schedules, compiled-state identity and observed frame timing. Do not hand-edit the GIFs or their provenance manifest.
- Public GIF URLs explicitly use the repository's raw GitHub host and a content-addressed revision directory. The release manifest maps each URL to the exact local reference bytes. Preserve previous revision directories in published history and when updating the served branch; do not overwrite older media with a new recording.
- Local packaging is not release approval. A release-equivalent full learner run with a verified fresh tutorial project must pass before publication, followed by a full learner run on the exact public tutorial URL before student distribution. `LEARNER-PLAYTESTER-V4` permits the existing supported browser and, when necessary, a strictly mechanical visible-action relay; a separate profile is not required.

See `THIRD_PARTY_NOTICES.md` and `LICENSES/MIT.txt` for source provenance and applicable notices.
