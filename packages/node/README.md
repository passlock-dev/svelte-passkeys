<div align="center">
  <a href="https://github.com/passlock-dev/ts-clients">
    <img src="https://github.com/passlock-dev/passkeys-frontend/assets/208345/53ee00d3-8e6c-49ea-b43c-3f901450c73b" alt="Passlock logo" width="80" height="80">
  </a>
</div>

<div>
  <h1 align="center">Passkeys, Social Login & more <br /> for Node.js apps</h1>
  <p align="center">
    Node SDK for Passkey authentication, Social Login using Apple, Google and more...
    <br />
    <a href="https://passlock.dev"><strong>Project website »</strong></a>
    <br />
    <a href="https://github.com/passlock-dev/ts-clients">GitHub</a>
    ·    
    <a href="https://passlock.dev/#demo">Demo</a>
    ·
    <a href="https://docs.passlock.dev">Documentation</a>
    ·
    <a href="https://docs.passlock.dev/docs/tutorial/introduction">Tutorial</a>
  </p>
</div>

<br />

## See also

For frontend usage please see the accompanying [@passlock/client][client] package

## Requirements

Node 16+

## Usage

Generate a secure token in your frontend then use this API to obtain the passkey registration or authentication details:

```typescript
import { Passlock } from '@passlock/node'

const passlock = new Passlock({ tenancyId, apiKey })

// token comes from your frontend
const principal = await passlock.fetchPrincipal({ token })

// get the user id
console.log(principal.user.id)
```

[contact]: https://passlock.dev/contact
[client]: https://www.npmjs.com/package/@passlock/client