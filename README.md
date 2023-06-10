This is a self-contained simplified version of the Azure ML examples repository, designed to show how training pipelines can be triggered on commits to the repo through GitHub actions.

The GitHub actions workflow is implemented for the `nyc-taxi` regression problem. 

Existing Github action runs (that were run on this code repo) can be accessed in the `Actions` of the repo. 

To replicate the GitHub actions workflow, follow [these steps](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-github-actions-machine-learning?view=azureml-api-2&tabs=userlevel). Note that you will need to add your Azure credentials as `secrets` to the repo as the variable `AZURE_CREDENTIALS`. This variable needs to be referenced in the `cli-jobs-pipelines-nyc-taxi-pipeline.yml` file that defined the GitHub action in `.github/workflows/cli-jobs-pipelines-nyc-taxi-pipeline.yml` (there is a mismatch here in the original repo).