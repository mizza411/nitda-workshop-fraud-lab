# Workshop polls (Firebase Firestore) — separate from the lab

The lab under `workshop_deck/practical/` stays as it is. This folder hosts two live polls on the same Firebase project.

## Public pages

Opening trust poll (ice-breaker):

- Vote: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/open.html
- Projector: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/open_results.html

Verdict poll (after lab checks):

- Vote: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/poll.html
- Projector: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/results.html

## Project

- Firebase project: `nitda-workshop-verdict`
- Store: Cloud Firestore (free tier)
- Config file: `firebase_config.json` (web client keys only)
- Opening session: `openingSessionId` (default `workshop-opening`)
- Verdict session: `sessionId` (default `workshop-default`)

## Reset votes before a session

In Firebase console → Firestore → delete documents under:

- `polls/workshop-opening/counts` (opening)
- `polls/workshop-default/counts` (verdict)

Or change the session ids in `firebase_config.json` and republish that file.

## CLI note (this PC)

Use `NODE_TLS_REJECT_UNAUTHORIZED=0` or `NODE_OPTIONS=--use-system-ca` with the tools under `C:\temp\fbtools` if TLS intercept breaks `firebase` API calls. Browser login can succeed while API calls still fail without that flag.

No Slido. No Mentimeter required.
