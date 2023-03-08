# test-deploy-hugo-pages-using-actions

![deploy workflow](https://github.com/thomaslaurenson/est-deploy-hugo-pages-using-actions/actions/workflows/deploy.yml/badge.svg)

```
hugo new site test-deploy-hugo-pages-using-actions
cd test-deploy-hugo-pages-using-actions
git init
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
echo "theme = 'PaperMod'" >> config.toml
hugo server
```
