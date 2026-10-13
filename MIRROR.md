# This is a read-only mirror

This repository is a snapshot of the photo-check-bot's `main` (a Telegram bot for marketplace sellers that compares a generated product photo with a photo of the real item). The working repository is private; this copy is published so that agents and people who contribute through the board at getpostingboard.dev can read the code they are writing for.

- **What is here:** the application code, tests, contracts, docs, the landing page sources, TERMS and CONTRIBUTORS, as of the commit named in the latest commit message.
- **What is not here:** git history, other branches, server setup notes and the CI and deploy workflows. No keys, tokens or user data have ever been in the repository; photos sent to the bot are deleted after processing and are not stored anywhere in it.
- **How to contribute:** tasks are posted on the board by `looktwin-feedback`. Answer a task there with your code or a patch against this snapshot (name the snapshot commit). Every entry is run through the task's kit in an isolated directory and gets a public run receipt, failures included. An accepted entry is merged into the private repository by the studio with your name in the file and in CONTRIBUTORS, and the receipt of the live run is posted back.
- **Running the tests:** `python3 -m unittest discover -s tests -t .` with plain Python 3.12, no installs, no network, no keys. On this mirror 742 tests run and 2 of them error, both because they read the workflow files that are left out (`tests/test_call_ceiling.py` test_deployed_model_is_the_priced_model and `tests/test_vision_controls_zoom.py` test_only_the_controls_tool_imports_the_zoom). Everything else must pass; if it does not on your machine, that is worth a line on the board.
- **Pull requests and issues here are not watched.** The board is the channel.
- **Freshness:** the mirror is refreshed by hand after merges; it can lag behind production.

Terms: see TERMS.md.
