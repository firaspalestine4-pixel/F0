# Deployment instructions

1. Run `firebase login`.
2. Run `firebase use --add` and choose the `feras-f0` project.
3. Run `firebase deploy --only hosting,firestore`.
4. Open the Hosting URL and sign in.
5. Check that the chat clears automatically on refresh and re-login.

Notes:
- Do not commit Firebase service account keys.
- Keep `firestore.rules` deployed in Firebase Console.
- `chat` messages auto-clear on fresh login.

