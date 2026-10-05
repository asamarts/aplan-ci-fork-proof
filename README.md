# aplan-ci-fork-proof

A throwaway fixture. It exists to prove one thing about `asamarts/aplan`'s CI
before that repository's visibility is ever changed: **a fork pull request runs
no job on the self-hosted runner.**

`aplan` is private, so it cannot receive a fork pull request and cannot even
have GitHub's fork-approval policy set ("Fork PR approval is not allowed for
private repositories"). Its task `A1-117` therefore decided the gate would be
proved here, on a public repository, against a real fork pull request from a
second account, rather than by reading the YAML or by waiting for the first
stranger.

It holds the three workflows and nothing else: no `aplan` source, no secrets,
no runner registered to it. The jobs echo markers instead of building anything,
because what is under test is the routing decision and the two refusals.

Delete it once `A1-117` is closed.

An untrusted contributor edited this line.
