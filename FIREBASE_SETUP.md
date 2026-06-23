# Fieldday Firebase signup setup

The website signup form writes emails to a Firestore collection named `launchSignups`.

1. In Firebase Console, create or open the Fieldday project.
2. Go to Project settings > General > Your apps, create/select a Web app, and copy the SDK config values.
3. Paste those values into `firebase-config.js` next to `index.html`.
4. In Firestore Database, create a database if one does not exist.
5. In Firestore Rules, publish the rules from `firestore.rules`.
6. Open the website, submit a test email, then confirm a document appears in `launchSignups`.

The Firebase web config is safe to be public. The Firestore rules are what prevent visitors from reading the list or writing outside the launch signup shape.