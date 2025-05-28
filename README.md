### Example Dependency submission snaphot upload command using the GH CLI

```
gh api \
  --method POST \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  /repos/callmegreg-demo-org/another-java-repo/dependency-graph/snapshots \
  --input create-deps-new-repo.json
```

### Example dependency submission payloads

- Creating a new dependency for a `pom.xml` file stored in the root of the repo
- Clearing out existing dependencies for a `pom.xml` file stored in the root of the repo

> [!NOTE]
> Using the same job `correlator` and detector `name` values, along with a more recent `scanned` timestamp, will overwrite existing dependencies for that same pair.
