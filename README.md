# Fjordova.ai for Gemini CLI

Ask Gemini CLI about your Fortnox books and let it propose changes. Nothing changes until the proposal is confirmed at your company's confirmation level. Sign in with your own Fortnox account.

Published by Gobrand och Borggren AB (559605-3032). Support: support@fjordova.com.

## Install

Install the extension in Gemini CLI:

```sh
gemini extensions install https://github.com/Fjordova-AB/fjordova-gemini
```

Restart Gemini CLI, then authenticate when prompted. You can also start sign-in with:

```text
/mcp auth fjordova
```

Select the intended Fortnox company. Available tools depend on your company's modules and your Fortnox permissions. Review proposed changes before confirming them.

## Try it

- Which customer invoices are overdue, and what is the total outstanding amount?
- Summarize the information available for my selected Fortnox company.
- Propose a customer update and show me the preview before it is confirmed.

## Connection

This extension connects to the hosted Fjordova MCP service at https://mcp.fjordova.ai/fortnox/mcp using OAuth. It contains no API keys, passwords or backend source code. Gemini CLI tool confirmations remain enabled.

## Compatibility

This package targets Gemini CLI, not the Gemini consumer chat app. Gemini CLI installation, OAuth and tool calls have not yet been independently verified for this package. Gallery availability depends on Google's indexing and validation.

## Links

- [Website](https://fjordova.ai)
- [Setup and support](https://fjordova.ai/koppla)
- [Privacy policy](https://fjordova.ai/integritetspolicy)
- [Service terms](https://fjordova.ai/villkor)
- [Gemini CLI extensions](https://geminicli.com/docs/extensions/)
