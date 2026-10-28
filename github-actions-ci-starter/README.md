# Beginner GitHub Actions CI Example

This tiny project runs two Python unit tests automatically whenever you push code to GitHub.

## Steps

1. Create/sign in to a GitHub account at https://github.com.
2. Create a **new repository**. Name it `github-actions-ci-starter`.
3. Download and unzip this project on your computer.
4. In the new GitHub repository, choose **Add file → Upload files**.
5. Upload the files and folders from inside this unzipped folder. Make sure `.github/workflows/ci.yml` is included.
   - If `.github` is hidden on your computer, enable hidden files in File Explorer.
6. Enter a commit message such as `Add first CI workflow`, then click **Commit changes**.
7. Open the repository's **Actions** tab. Click **Python CI** and open the latest run.
8. Wait for the green check mark and `success`.
9. To capture the requested screenshot, take a screenshot of that successful run page. On Windows, press **Win + Shift + S**, select the page, and save the image.
10. To save the logs, open the successful run, click the `test` job, and use the download-logs option (usually in the run page's menu) or copy the visible log text.

## What the workflow does

- Downloads the repository code.
- Installs Python 3.12.
- Runs the tests in `tests/`.
- Marks the run as failed if any test fails.

## Run the tests on your computer (optional)

Install Python 3.12 from https://www.python.org/downloads/, open a terminal in this folder, and run:

```bash
python -m unittest discover -s tests -v
```

The sample log file included in this project is illustrative only. It is **not** a log from a real GitHub Actions run.
