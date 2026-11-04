# flluter5

Flutter application is in [`secure_http/`](./secure_http/).

## Run in a local browser

Install Flutter, then run these commands from the project directory:

```powershell
cd secure_http
flutter pub get
flutter run -d chrome
```

The login is simulated: enter any valid email address and a non-empty password.
A dummy token is saved in browser secure storage. This is for practice only and
does not authenticate a real account.

## Publish on GitHub Pages

The workflow in `.github/workflows/deploy-pages.yml` builds the web app and
publishes it at:

<https://bintangandaraputra.github.io/flluter5/>

In the repository, open **Settings → Pages** and set **Build and deployment →
Source** to **GitHub Actions**. Push to `main` (or run the workflow manually
from the **Actions** tab) to build and deploy.

The Pages build uses HTTPS, which is required for browser secure storage.
GitHub Pages is static hosting; real account authentication requires a backend
and is not part of this simulated-login exercise.
