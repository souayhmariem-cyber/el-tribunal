# Contributing to El Tribunal

## Working agreements

- Work on a focused branch; do not commit feature work directly to `main`.
- Keep pull requests small and describe the motivation, scope, and verification performed.
- Do not merge a pull request until it has been reviewed.
- Avoid adding dependencies unless the change needs them; explain the choice in the pull request.
- Keep shared API contracts explicit and version changes coordinated between client and server.

## Case-material handling

- Never place creator-only case truth, answer keys, hidden motives, scoring keys, or unreleased solutions in `client/`, frontend public assets, or any browser-delivered bundle.
- Only approved player-safe case content may be delivered to the client.
- Do not alter original creator source files as part of routine implementation.
- Do not commit credentials, personal data, real incident records, or production datasets.

## Engineering expectations

- Validate all untrusted input on the server.
- Enforce authorization and investigation ownership on every protected API operation.
- Keep scoring and answer evaluation server-side.
- Make the 3D scene a visualization of backend-owned state, not the source of truth.
- Add or update tests when introducing behavior.
- Document significant architecture or API decisions in `docs/`.

## Pull request checklist

- [ ] Scope is focused and matches the issue.
- [ ] No secrets or creator-only case content are included.
- [ ] Validation and authorization are handled where relevant.
- [ ] Tests or manual verification are described.
- [ ] Documentation is updated where needed.
