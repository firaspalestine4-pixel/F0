# F0 deployment checklist

## Files

- `index.html` — application entry point
- `logo.png` — application logo
- `firestore.rules` — authenticated chat access rules
- `firebase.json` — Firebase Hosting and Firestore configuration

## Deploy with Firebase CLI

From the repository root:

```bash
firebase login
firebase use feras-f0
firebase deploy --only hosting,firestore
```

If the project is not linked locally, run `firebase use --add` and select `feras-f0`.

## Verify after deployment

1. Open the deployed Hosting URL.
2. Sign in with an existing account.
3. Confirm the chat loads.
4. Send a message of fewer than 500 characters.
5. Confirm the message appears after refreshing.
6. Sign out and confirm the protected screens are no longer accessible.

Never place Firebase service-account private keys in this repository or in `index.html`.
