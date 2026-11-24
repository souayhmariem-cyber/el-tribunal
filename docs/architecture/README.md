# Architecture

## Current direction

El Tribunal uses one reusable investigation engine configured by five independent cases. The cases do not depend on a shared narrative or cross-case progression.

## Core boundaries

- **Client:** presentation, interaction, and 3D visualization.
- **Server:** authentication/authorization, case access, evidence unlocks, investigation state, hypotheses, response validation, scoring, and report evaluation.
- **Database:** durable users, case versions, investigations, evidence access, events, hypotheses, responses, and results.
- **Shared:** safe API contracts and types only. Never put answer keys or creator-only truth here.

## Non-negotiable security boundary

The backend owns game truth and evaluation. The client receives only player-safe content and authorized state. Creator-only content and grading rules remain server-side and must not be bundled into frontend code.

## Implementation status

This document records the agreed direction; detailed component, deployment, and threat-model decisions remain to be specified before implementation.
