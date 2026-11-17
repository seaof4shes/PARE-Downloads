# P.A.R.E. Download Website

This repository contains only the public static website for P.A.R.E. It does not contain the Flutter application source code.

## Before publishing

1. Open `index.html`.
2. Find `YOUR-GITHUB-USERNAME`.
3. Replace it with your GitHub username.
4. Save the file.

## Publish with GitHub Pages (free on GitHub Free for public repositories)

1. Create a **new public repository** named `PARE-Downloads`.
2. Upload `index.html`, `style.css`, and `README.md` to the repository root.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then click **Save**.
6. Wait for the deployment to finish. Your site address will be:
   `https://YOUR-GITHUB-USERNAME.github.io/PARE-Downloads/`

## Publish the APK separately using GitHub Releases

1. Open the `PARE-Downloads` repository.
2. Select **Releases → Create a new release**.
3. Create a tag such as `v1.0.14` (use the actual version you intend to publish).
4. Add release notes.
5. Attach your APK file as a release asset.
6. Publish the release.

The website's button points to:
`https://github.com/YOUR-GITHUB-USERNAME/PARE-Downloads/releases/latest`

The button opens the latest release page, where visitors can select the APK asset.

## Keep the Flutter source private

- Do not upload your Flutter project, `lib/`, `android/`, model files, Firebase configuration, signing keys, or secrets to this public website repository.
- Keep your existing `pare_app` repository private.
- Only upload the final APK you intend to distribute as a release asset.
- A public APK can be downloaded and inspected/reverse-engineered; keeping source code private does not make the compiled app impossible to analyze.

## Updating later

For a new APK, create another GitHub Release with a new version tag and attach the new APK. The website's `/releases/latest` link will continue to open the newest release.
