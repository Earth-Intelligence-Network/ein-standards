# EIN standards

The open standards of the Earth Intelligence Network (EIN): the event kinds, wire formats, profiles and test vectors
that let any app or node take part in the network without asking anyone. Licensed Apache-2.0, so anyone may
implement them, in any language, under any licence.

## Status: being set up

The standards live today in Starcom's repository, in
[`docs/spec/`](https://github.com/Starcom-Platform/starcom/tree/main/docs/spec), where
[`docs/spec/README.md`](https://github.com/Starcom-Platform/starcom/blob/main/docs/spec/README.md) says where to start.
They will move here; no date is set. Starcom will then read a pinned version from here, like any other
implementation, so the network's rules belong to the network and not to one app.

## What will be here

- **The event kinds,** as data: every kind the network's apps and nodes use, and what each does with it.
- **The specs:**
  - the interchange of Mission Packages, findings, refutations, roster items and globe notes;
  - attested claims, a draft NIP;
  - the share handle;
  - the globe intelligence layer;
  - harm accounting.
- **Four profiles,** saying what an app or node must do to claim each:
  - **Reader:** reads by place and time, weighs claims by their method and sources, and honours withdrawals.
  - **Publisher:** signs, places notes no more precisely than it was given, and shows people what goes before it goes.
  - **Node:** a relay, archive, mirror, indexer or curator that describes itself.
  - **Agent:** an AI publisher with an operator of record.

  A profile describes; it never grants permission.
- **Test vectors** for each, with reference checkers that import no app's code.
- **How a standard changes,** proposed so far:
  - a new idea starts in its own namespace;
  - it becomes a standard once two independent implementations use it;
  - a breaking change needs three independent implementations to agree, and six months' notice.

## Taking part

- Read the specs where they are now, and run their vectors (`npm run conformance` in Starcom).
- Propose a change or report a contradiction in an issue here.
- Implementations so far: [Starcom](https://github.com/Starcom-Platform/starcom), the reference frontend.
