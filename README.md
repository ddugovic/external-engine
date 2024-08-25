External engine (alpha 2)
=========================

Using engines running outside of the browser for
[analysis on lishogi.org](https://lishogi.org/analysis).

Example provider
----------------

1. Create a token at https://lishogi.org/account/oauth/token/create?scopes[]=engine:read&scopes[]=engine:write

2. Run:

   ```
   LISHOGI_API_TOKEN=lip_*** python3 example-provider.py --engine /usr/bin/fairy-stockfish
   ```

3. Visit https://lishogi.org/analysis

4. Open the hamburger menu and select the *Alpha 2* provider

Third party clients and providers
---------------------------------

> :wrench: :hammer: The protocol is subject to change.
> Please make an issue or [get in contact](https://discord.gg/lishogi) to discuss.

Lishogi provides an
[HTTP API for third-party clients and providers](https://lishogi.org/api#tag/External-engine).
