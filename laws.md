# Engineering Laws

The rules every change in this project must follow.

---

## ENG-4.1 — Atomic TDD

**In simple words:** write the failing test first, make it pass with the smallest code, and commit each behavior on its own.

- **Red:** write a test for the new behavior and watch it fail.
- **Green:** write the smallest amount of code that makes the test pass.
- **Refactor:** clean up while keeping all tests green.
- **Commit:** one behavior per commit. Don't bundle unrelated changes.

---

## ENG-5.2 — CI/CD Pipeline

**In simple words:** code reaches users only through the automated pipeline. No manual deploys, no skipped stages.

- Every change goes through the pipeline: build → test → deploy.
- No deploying by hand from a local machine.
- No skipping or disabling stages to get a change out faster.
- If a stage fails, fix the cause rather than bypassing the stage.

---

## ENG-6.1 — Security by Design

**In simple words:** build security in from the first line. Check ownership, validate input, protect secrets.

- **Check ownership:** confirm that the current user owns or is allowed to access each resource before reading or changing it.
- **Validate input:** treat all external input as untrusted, and validate it at the boundary.
- **Protect secrets:** never hard-code or commit keys, tokens or passwords. Load them from environment variables or a secret manager.