# tournament-signup

The player sign-up page for Tournament-App's QR check-in.

The organizer's app shows a QR code that opens this page with a random channel name in the link. The player types their name, and the page sends it through [ntfy.sh](https://ntfy.sh) (a free relay, no account needed) to the organizer's app, where the organizer approves it into the player list.

This repo only holds this one static page and is public so it can be hosted free on GitHub Pages. The app itself lives in a separate private repo.

Live at: https://nzimmer-apps.github.io/tournament-signup/
