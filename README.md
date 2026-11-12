# tournament-signup

Public pages for Tournament-App. The player sign-up page for Tournament-App's QR check-in.

The organizer's app shows a QR code that opens this page with a random channel name in the link. The player types their name, and the page sends it through [ntfy.sh](https://ntfy.sh) (a free relay, no account needed) to the organizer's app, where the organizer approves it into the player list.

It also hosts the **live viewer** in [`live/`](live/): the page players and venue TVs open from the organizer's live link. It receives signed, display-only updates from the organizer's app through the same relay, and checks each one's signature before showing it.

It also hosts the **browser version of the organizer app** in [`app/`](app/), for organizers on iPhone, laptop or tablet.

This repo only holds these static pages and is public so it can be hosted free on GitHub Pages. The app itself lives in a separate private repo.

- Sign-up: https://nzimmer-apps.github.io/tournament-signup/
- Live viewer: https://nzimmer-apps.github.io/tournament-signup/live/ (needs the full link from the app)
- Organizer app: https://nzimmer-apps.github.io/tournament-signup/app/

The live viewer and web app files are built in the private app repo (`npm run build:viewer`, `npm run build:web`) and copied here.
