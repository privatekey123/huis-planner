# MovePlanner

MovePlanner 2.0 source has been uploaded to this repository as an import archive because direct `git push` from the current workspace is blocked.

## Finish Import

Open the GitHub Actions workflow and run it once manually:

https://github.com/privatekey123/huis-planner/actions/workflows/import-moveplanner-chunks.yml

Choose **Run workflow** on branch `main`. The workflow reassembles the uploaded source chunks, extracts the Swift macOS project, removes the temporary chunk files, and commits the full MovePlanner project to `main`.

Expected imported project files include:

- `Package.swift`
- `Sources/MovePlanner/*.swift`
- `Assets/MovePlannerLogo.svg`
- `Scripts/build-app.sh`
- `Support/MovePlannerInfo.plist`

If the workflow cannot push its result, enable GitHub Actions write permissions for the repository and run it again.