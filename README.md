Example Dependency submission snaphot upload:

```
gh api \
  --method POST \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  /repos/callmegreg-demo-org/another-java-repo/dependency-graph/snapshots \
  --input create-deps-new-repo.json
```
