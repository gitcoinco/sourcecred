# DemoData Instructions

This folder contains example data for testing the GitHub plugin. The example
data is generated by running our GitHub API fetch against the SourceCred
example repo at https://github.com/sourcecred-test/example-github/.

The demo data should be regenerated any time either the example repository or
the GitHub api query changes. To regenerate the demo data, you can run the general-purpose
snapshot updater:

```shell
$ SOURCECRED_GITHUB_TOKEN="your_token_here" scripts/update_snapshots.sh
```

There is a known issue where GitHub's end cursor output depends on your current
timezone. The example data is canonically generated from the US/Pacific
timezone.
