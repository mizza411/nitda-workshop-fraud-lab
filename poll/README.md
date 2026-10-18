# Workshop polls (Firebase Firestore) — separate from the lab

The lab under `workshop_deck/practical/` stays as it is. This folder hosts live polls on the same Firebase project.

## Public pages

Opening trust poll Q1:

- Vote: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/open.html
- Projector: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/open_results.html

Opening worry poll Q2:

- Vote: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/open2.html
- Projector: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/open2_results.html

Spot the shop poll (after lab checks):

- Vote: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/poll.html
- Projector: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/results.html
- Options: Trust / Doubt / Walk away
- Session: `sessionId` (default `workshop-spot-shop`)

## Project

- Firebase project: `nitda-workshop-verdict`
- Store: Cloud Firestore (free tier)
- Config file: `firebase_config.json` (web client keys only)

## Reset votes before a session

In Firebase console → Firestore → delete documents under the relevant `polls/{session}/counts` path, or change the session ids in `firebase_config.json` and republish that file.

No Slido.
