# Spinup

> Spinup gives cloud agents an identity, a runtime, and an operating history.

Most agents are a prompt and a webhook. Once an agent needs files, packages, browsers, secrets, and state across runs, the runtime stops being an implementation detail. So does the question of who the agent is, what it's allowed to do, and what it did last week.

Spinup is the layer that makes both answerable.

This org holds the code and docs behind that.

We're early. The public surface is small on purpose.

## What you get per agent

- A durable identity owned by your workspace
- An isolated environment with its own filesystem, packages, tools, and state
- Skills, secrets, and a network policy attached to that identity
- Snapshots for pause, restore, replace
- A swappable harness inside the environment (OpenClaw, Hermes, more coming)
- Run history that survives harness and machine changes
- Suspend, revoke, or delete at the agent level

## Why the identity layer

Agent identity is the durable object. Models change. Harnesses change. The machine underneath gets recycled. What survives is the agent: who owns it, what it can do, what it did, how to revoke it.

That's the layer Spinup is building.

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
