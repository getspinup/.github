# Spinup

Spinup is building the runtime layer for agents that need more than a model call.

Files. Packages. Browsers. Secrets. State. Once an agent needs those, the runtime stops being an implementation detail.

This org is for the code behind that.

We're early. The public surface is small on purpose.

## What Spinup is

- A cloud agent runtime
- One isolated environment per agent
- A stable API above the runtime
- Swappable harnesses inside the same agent model
- Agent-level skills, secrets, network policy, and snapshots

## Start here

- [`Docs`](https://www.getspinup.com/docs): public docs home
- [`Getting Started`](https://www.getspinup.com/docs/getting-started): the product model and access paths
- [`CLI`](https://www.getspinup.com/docs/cli/install): install `spinup` and log in
- [`SDK`](https://www.getspinup.com/docs/sdk/typescript): use `@getspinup/sdk` from code
- [`Runtime API`](https://www.getspinup.com/docs/agent-api/authentication): authenticate to a live agent

## What lives in the monorepo

- Web app and API
- CLI and SDK
- Auth, contracts, and database code
- Execution plane, worker host, supervisor, and provisioning path

## Who this is for

Developers building agent products that need isolation, persistence, tools, and sane runtime controls.

If your agent is basically a prompt plus a webhook, this will probably feel like overkill.
If it behaves like a small computer, you are in the right place.

[Docs](https://www.getspinup.com/docs)
