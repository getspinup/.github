# Spinup

> A cloud agent runtime. One agent. One computer. Any harness.

Each agent gets its own cloud computer: files, packages, browsers, secrets, and state that persist between runs. The harness on top is swappable. The agent underneath is workspace-owned, with a stable ID and a kill switch.

Spinup is the runtime that future agent names will point at. The first step toward agent identity.

This org holds the code and docs behind that.

The public surface is small on purpose.

## What you get per agent

- An isolated cloud computer with its own filesystem, packages, tools, and state
- A workspace-owned agent with a stable ID, owner, and lifecycle
- Skills, secrets, and a network policy attached to the agent
- Snapshots for pause, restore, replace
- A swappable harness inside the environment (OpenClaw, Hermes, more coming)
- Run history that survives harness and machine changes
- Suspend, revoke, or delete at the agent level

## Why a runtime

Build the agent once. Run it on a real cloud computer. Swap the harness when the ecosystem changes.

Models change. Harnesses change. The machine underneath gets recycled. What survives is the agent: who owns it, what it can do, what it did, how to revoke it.

Identity, history, and tool portability come with the runtime.

## Start here

- [`Docs`](https://www.getspinup.com/docs): public docs home
- [`Getting Started`](https://www.getspinup.com/docs/getting-started): the product model and access paths
- [`CLI`](https://www.getspinup.com/docs/cli/install): install `spinup` and log in
- [`SDK`](https://www.getspinup.com/docs/sdk/typescript): use `@getspinup/sdk` from code
- [`Runtime API`](https://www.getspinup.com/docs/agent-api/authentication): authenticate to a live agent

## Current focus

- Web app and API
- CLI and SDK
- Auth, contracts, database
- Execution plane: worker host, supervisor, Firecracker provisioning

## Who this is for

Developers and teams building agents that behave like small computers and that someone has to be accountable for.

If your agent is a prompt plus a webhook, this will feel like overkill.
If it runs for minutes, touches files, holds credentials, or has to be revocable, you're in the right place.

[Docs](https://www.getspinup.com/docs)
