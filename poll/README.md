# Verdict poll (Firebase Firestore) — separate from the lab

The lab under `workshop_deck/practical/` stays as it is. This folder is only the shared Match / No match / Walk away tally.

## Public pages

- Vote: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/poll.html
- Projector: https://mizza411.github.io/nitda-workshop-fraud-lab/poll/results.html

## Project

- Firebase project: `nitda-workshop-verdict`
- Store: Cloud Firestore (free tier)
- Config file: `firebase_config.json` (web client keys only)

## Reset votes before a session

In Firebase console → Firestore → delete documents under `polls/workshop-default/counts`, or change `sessionId` in `firebase_config.json` and republish that file.

## CLI note (this PC)

Use `NODE_TLS_REJECT_UNAUTHORIZED=0` or `NODE_OPTIONS=--use-system-ca` with the tools under `C:\temp\fbtools` if TLS intercept breaks `firebase` API calls. Browser “Woohoo” login can succeed while API calls still fail without that flag.
