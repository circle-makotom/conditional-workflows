# tl;dr

`curl -X POST -H "Circle-Token: $YOUR_API_KEY" -H "Content-Type: application/json" -d '{"parameters":{"do-deploy":true}}' https://circleci.com/api/v2/project/github/circle-makotom/conditional-workflows/pipeline` will:

* trigger the `alert-deploy` workflow
* let the `deploy` job do deployment, and
* execute the conditional steps in the `build` job
