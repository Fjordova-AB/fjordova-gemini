# Fjordova för Gemini CLI

Fråga Gemini CLI om din bokföring och låt den föreslå ändringar via Fjordova. Förslag bekräftas enligt företagets bekräftelsenivå. Logga in med ditt eget Fortnox-konto.

Utgivare: Gobrand och Borggren AB (559605-3032). Support: support@fjordova.com.

## System som stöds

Den generella Fjordova-adressen ger i dag åtkomst till **Fortnox**. Spiris är ännu inte tillgängligt via den här adressen.

Du behöver ett Fortnox-konto och åtkomst till det företag och de moduler du vill använda. Tillgängliga verktyg beror på företagets valda moduler, licenser och dina Fortnox-behörigheter.

## Installera

Installera tillägget i Gemini CLI:

```sh
gemini extensions install https://github.com/Fjordova-AB/fjordova-gemini
```

Starta om Gemini CLI och logga in när du blir ombedd. Du kan också starta inloggningen med:

```text
/mcp auth fjordova
```

Välj rätt Fortnox-företag. Läs varje ändringsförslag innan du bekräftar det.

## Prova

- Vilka kundfakturor är förfallna och vad är det totala utestående beloppet?
- Sammanfatta den tillgängliga informationen om mitt valda Fortnox-företag.
- Föreslå en kunduppdatering och visa förhandsgranskningen innan den bekräftas.

## Anslutning

Tillägget ansluter till Fjordovas MCP-tjänst på `https://mcp.fjordova.ai/mcp` med OAuth. Det innehåller inga API-nycklar, lösenord eller serverkod.

Har du redan en anslutning till `https://mcp.fjordova.ai/fortnox/mcp` behöver du göra en ny OAuth-anslutning för den generella adressen. Enbart ett URL-byte flyttar inte det tidigare samtycket. Kontrollera att den nya anslutningen fungerar innan du tar bort den gamla.

## Kompatibilitet och verifieringsstatus

Paketet är avsett för Gemini CLI. Det installerar ingen koppling i Geminis vanliga chattapp. Installation, OAuth-inloggning och verktygsanrop behöver verifieras med den generella adressen. Tillgänglighet i tilläggsgalleriet beror på Googles indexering och validering; repot innebär ingen bekräftad gallerilistning.

## Länkar

- [Webbplats](https://fjordova.ai)
- [Anslutning och support](https://fjordova.ai/koppla)
- [Integritetspolicy](https://fjordova.ai/integritetspolicy)
- [Tjänstevillkor](https://fjordova.ai/villkor)
- [Tillägg för Gemini CLI](https://geminicli.com/docs/extensions/)
