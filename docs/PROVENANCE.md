# Provenance

Date: 2026-10-12

- Upstream checkout named by `docs/navrl_upstream_diff_2026-03-27.md`: `/home/gwh/NavRL_upstream`
- Upstream exact commit: unknown/unresolved
- Canonical branch: `main` at `d2008c178088bb7c344d71f555edd53cf7f1fa65`

Git history, submodules, and that note do not record an upstream SHA. The note itself says this repository is a separate port, not an in-place edit. It changes the platform from the Hummingbird drone to DashGo, the action to local `[v, w]`, the observation layout, and the reward target.

Fidelity: F3. Those reward, observation, and action changes mean this tree is not a fair original NavRL baseline. The missing upstream SHA is not inferred.

Audited branch `codex/navrl-rootcause-fix-20260403` is `1320920735684bda5fa16bc18db1f079e3e8bc82`. Merge-base with `main` is `f54dcb14f45aa307f4be6286379dcc48fc7fb0dd`. It is 2 commits ahead (`751c03c`, `1320920`) and 1 behind (`d2008c1`). Unique paths include `src/navrl_dashgo/checkpointing.py`, `tests/test_checkpointing_resume.py`, and `tools/watch_background_train_until.py`. It was not merged: it diverges from `main`, and the training utilities were not rerun in this governance pass.
