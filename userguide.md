Set Up Documentation to Deploy as Part of the Workflow

Fork this repo: https://github.com/linuxacademy/content-github-actions-deep-dive-lesson. Check out the lab branch.

You can clone the repo locally or use the GitHub interface. Check the /.github/workflows/pipeline.yaml file. The workflow contains jobs to run a linter and build an artifact. Create a docs directory and a userguide.md file at the root directory. Add some text to the file and save it.

Add a job to the workflow to deploy the user guide file to GitHub Pages. This is an instance where a Community Action might save some time. Check the Pages URL to confirm the Markdown has been converted to html and published.

et Up a Trigger Condition for the Workflow

The docs are deploying with the pipeline, but the file hasn't been updated in the last few commits, leading to the docs still being out of date. Add a condition so the workflow doesn't run unless the user guide has been changed — that way, new code won't build without supporting documentation.

Update the user guide and push the changes to validate that the new changes have deployed.

Update the code file without changing the user guide and push those changes. Verify that the workflow doesn't run without updates to the docs.
