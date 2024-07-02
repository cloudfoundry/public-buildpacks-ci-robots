# Introduction

This contains the state for the Cloud Foundry Buildpacks team [Concourse deployment](https://buildpacks.ci.cf-app.com/).

# Directories

* [binary-builds-new](binary-builds-new) Contains published metadata for each dependency version/compatible stack combination built by the [dependency-builds pipeline](https://buildpacks.ci.cf-app.com/teams/main/pipelines/dependency-builds).

* [binary-verification-whitelist](binary-verification-whitelist) Every day we verify that binaries being distributed via buildpacks.cloudfoundry.org have the correct checksums. Some binaries are, due to development error, known to be wrong. This branch is a list of files to ignore during verification.

* [new-cve-notifications](new-cve-notifications) Tracks CVEs and sorts them based on whether they affect the cflinuxfs3 rootfs

* [receipt-diffs](receipt-diffs) Used to determine whether to automatically release a new version of cflinuxfs* stacks