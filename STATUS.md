# Status

Updated 2026-11-03. Version 1.1.0 is a candidate using Fjordova's shared MCP endpoint: `https://mcp.fjordova.ai/mcp`.

- The public manifest description and README are in English and describe Fjordova independently of a particular business system.
- Package validation covers JSON, the MCP endpoint, the preserved `trust: false` setting and whitespace checks. This is not a live authentication test.
- The existing extension ID, version and MCP server key are preserved.
- Installation in Gemini CLI, OAuth sign-in and live tool calls through the shared endpoint remain unverified.
- Shared Spiris gateway and reviewer-flow implementation in Fjordova PRs #201 and #202 was merged on 2026-11-03. Production deployment, activation and end-to-end access are not verified by this package update.
- Fortnox is the existing production integration. Spiris, Bolagsverket and other integrations are not claimed as available through this connector without production evidence.
- The changes are prepared for existing draft PR #1. Updating that branch does not change main or the gallery. The default installation still uses main until the PR is merged; candidate verification must use the PR branch.
- No marketplace approval or publication is established by this package. The extension targets Gemini CLI, not the Gemini chat app.

Next: review and update the existing PR, verify the deployed shared gateway, then test fresh OAuth, company selection, tool discovery, a read-only call and token refresh in Gemini CLI before considering the candidate ready for publication or indexing.
