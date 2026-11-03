# Fjordova for Gemini CLI

Connect Gemini CLI to the business systems and data sources enabled for your Fjordova account. Ask questions about the data you can access and, where supported, prepare changes for review. Proposals follow your company's selected confirmation level before execution.

Publisher: Gobrand och Borggren AB (559605-3032). Support: support@fjordova.com.

## Availability

The shared Fjordova MCP endpoint is `https://mcp.fjordova.ai/mcp`.

Fortnox is the existing production integration. Spiris and additional sources, including Bolagsverket, must not be considered available through this connector until production activation and end-to-end access have been verified. Installation, OAuth sign-in and tool calls from Gemini CLI through the shared endpoint are still awaiting verification.

The tools you can use depend on your connected systems, selected company, enabled modules, licences and permissions. A shared URL does not grant access to an unconnected system.

## Install

The shared-endpoint candidate is in [pull request #1](https://github.com/Fjordova-AB/fjordova-gemini/pull/1), on branch `codex/generell-mcp-20261101`. Until that change is merged, the default installation below uses `main` and does not include this candidate. For candidate verification, use the PR branch and check its manifest before installation; a default installation is not evidence that the shared endpoint works.

Install the extension in Gemini CLI:

```sh
gemini extensions install https://github.com/Fjordova-AB/fjordova-gemini
```

Restart Gemini CLI and sign in when prompted. You can also start authentication with:

```text
/mcp auth fjordova
```

Check the selected company and granted access. The extension uses OAuth and contains no API keys, passwords or server code.

If you have an older system-specific connection, create a new OAuth connection for the shared endpoint. Changing a URL does not transfer the previous authorization. Check that the new connection works before removing the old one.

## Try it

- Which company and connected systems can I access?
- Summarize the information available for my selected company.
- If supported, prepare a proposed customer update and show the preview without executing it.

Review each proposal before confirmation. Depending on your company's settings, the AI app may confirm a change after your approval in the conversation, or you may need to confirm it on a Fjordova page. Do not assume that every change requires a separate webpage confirmation.

## Compatibility and verification status

This extension is for Gemini CLI. It does not install a connector in the Gemini chat app.

This package is a candidate for the shared endpoint. Historical tests using a system-specific endpoint do not verify this connection. Availability in the extension gallery depends on Google's indexing and validation; the repository does not establish a gallery listing. See [STATUS.md](STATUS.md) for the current validation record.

## Links

- [Website](https://fjordova.ai)
- [Connection guide and support](https://fjordova.ai/koppla)
- [Privacy policy](https://fjordova.ai/integritetspolicy)
- [Terms of service](https://fjordova.ai/villkor)
- [Gemini CLI extensions](https://geminicli.com/docs/extensions/)
