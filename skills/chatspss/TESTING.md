# Test scope

On 2026-10-30 a Codex subagent explicitly read the upstream 0.2.2 SKILL.md and ran its packaged script with Python 3.13.14 on macOS arm64 against a synthetic 12-row CSV. The `overview` task completed with exit code 0 and empty stderr. The agent reproduced the complete Markdown table without a code fence and interpreted it, including that one missing income value gave N=11. The tested script SHA-256 was `15aa64efc8e5067ece4653eeaf83db9d32b47ea0ab49945ea8e118ddc25c51f2`.

This was explicit loading, not a test of automatic skill discovery. Claude, Copilot, Cursor, and VS Code have not been tested. One smoke test does not validate every analysis method or environment.
