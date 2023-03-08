# test-deploy-hugo-pages-using-actions

![deploy workflow](https://github.com/thomaslaurenson/test-deploy-hugo-pages-using-actions/actions/workflows/deploy.yml/badge.svg)

A repo to test building and deploying a Hugo project using GitHub Actions.


To copy the workflow, you need to configure GitHub pages using Actions for deployment first. To do this, in the target repo:

- Navigate to `Settings`
- Select `Pages`
- Under the `Build and deployment` section
- Set the `Source` section
- Set this to `GitHub Actions`

Then add the workflow as it appears in this repo in the `.github/workflows/deploy.yml` file.

Below is a summary of creating the Hugo project:

```
hugo new site test-deploy-hugo-pages-using-actions
cd test-deploy-hugo-pages-using-actions
git init
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
echo "theme = 'PaperMod'" >> config.toml
hugo server
```
