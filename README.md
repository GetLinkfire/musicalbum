# Music Albums Library — Take-Home Assignment

## Overview

Build a microservice that lets users manage a personal library of music albums. Album data comes from a third-party music catalogue (Spotify or Deezer).

We are not looking for a production-complete system — we are looking at how you structure one.

**Time budget:** Aim for about 4 hours of focused work. Please don't spend more than 6 — if you run short, keep the service and its unit tests complete, then the API test, then deployment, and write down in the README what you would have done next.

## Part 1 — The Service

Implement a microservice supporting the following:

**Users and libraries**
- A user is just a name — no other attributes, no profile.
- Each user owns exactly one library, and a library belongs to exactly one user.
- Authentication is not required, but is welcome if you want to show it.

**Search for albums**
- Search by album name and artist name.
- Back the search with either the Spotify API or the Deezer API.
- Each result should include: artist name, album name, album cover (when available), and album URL.

**Manage the library**
- Add one or more albums from search results to the library.
- Remove albums from the library.

**Test it**
- Include unit tests. We are not looking for 100% coverage — show us the parts you chose to make unit-testable, and why that shape works.

**Document it**
- A README with everything needed to build and run the service.

## Part 2 — API Test Automation

- Write an automated API test covering at least one endpoint.
- Use any test automation framework you are comfortable with.
- Include a README covering setup and execution, complete enough that we can run the suite without asking you questions.

## Part 3 — Deployment

Pick whichever of these you know best:

1. **Local folder** — publish the service locally and document how to run it plus any infrastructure it needs.
2. **Docker** — ship a `docker-compose` setup that brings up the service and its dependencies.
3. **Kubernetes** — deploy to a local cluster (Minikube, MicroK8s, kind). Share the YAML manifests and a README with deployment steps.

Whichever you choose, the README is part of the deliverable.

## Technical Requirements

- **.NET 10 or later.**
- Any third-party libraries or tools you like.
- The solution should be testable by design.

## Prerequisites

- .NET 10 SDK and an IDE of your choice (Visual Studio, VS Code, Rider).
- If you deploy to a container or cluster: Docker, and a local or cloud Kubernetes cluster for option 3.

## What We're Looking For

Two things, in roughly equal measure:

1. **The code itself** — structure, naming, error handling, test design, and the trade-offs you chose to make explicit.
2. **How you'd scale it** — assume we ship *both* Spotify and Deezer, and add more providers later. We're interested in how your design absorbs that: where the provider boundary sits, what stays the same when a third one arrives, and how you'd handle differences in their data and rate limits.

A short section in the README explaining your architectural decisions (and anything you deliberately left out) is worth more to us than extra features.

## Submitting

Share a link to a public Git repository, or a zip archive, containing the service, the API test project, deployment files, and READMEs.

## Notes

* Write this the way you would write code on a normal working day — same structure, same care, no need to gold-plate it.
* Use whatever stack you like for the API tests.
* Send us what you have when time is up even if the task is unfinished. An incomplete solution with a clear README beats a rushed complete one, and we would rather see where you got to than nothing at all.
* If anything in the task is ambiguous, make a decision, note it in the README, and move on.

**Choosing a provider.** Deezer is the lower-friction option: its public search endpoints need no API key, no app registration and no paid account, so you can call them straight away. Spotify requires registering an app in its developer dashboard for a client ID and secret, and its documentation states that the Web API expects a Spotify Premium account. Either provider is fine for this task — pick the one that gets you to the interesting part faster.

Questions are welcome at any point while you work on this — reach out and we will help.

## References

**Music APIs**
* [Spotify Web API](https://developer.spotify.com/documentation/web-api) — see the [getting started tutorial](https://developer.spotify.com/documentation/web-api/tutorials/getting-started) for registering an app and obtaining a client ID and secret
* [Deezer API](https://developers.deezer.com/api) — search endpoints are open; logging in is required to accept the terms for the wider API

**.NET**
* [.NET downloads](https://dotnet.microsoft.com/download) — .NET 10 is the current LTS release
* [.NET support policy](https://dotnet.microsoft.com/platform/support/policy/dotnet-core)

**IDEs**
* [Visual Studio 2026 (Community)](https://visualstudio.microsoft.com/vs/community/) — Windows
* [Visual Studio Code](https://code.visualstudio.com/) — Windows, macOS, Linux
* [JetBrains Rider](https://www.jetbrains.com/rider/) — Windows, macOS, Linux; free for non-commercial use

**Local Kubernetes**
* [MicroK8s](https://canonical.com/microk8s/)
* [minikube](https://minikube.sigs.k8s.io/docs/start/)
