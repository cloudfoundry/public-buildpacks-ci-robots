# Introduction

This contains the state for the Cloud Foundry Buildpacks team [Concourse deployment](https://buildpacks.ci.cf-app.com/).

# Directories

* [binary-builds-new](binary-builds-new) Contains published metadata for each dependency version/compatible stack combination built by the [dependency-builds pipeline](https://buildpacks.ci.cf-app.com/teams/main/pipelines/dependency-builds).

* [new-release-notifications](new-release-notifications) When a dependency included in a buildpack has a new version released, an update is made to this branch

* [binary-builds](binary-builds) Used to enqueue build jobs for both manual and automatic builds

* [binary-built-output](binary-built-output) When an automatic build finishes, it stores binary signatures and timestamps in this branch.


* [new-cve-notifications](new-cve-notifications) Tracks CVEs and sorts them based on whether they affect the cflinuxfs2 rootfs

* [resource-pools](resource-pools) Used to control access to the LTS BOSH-lite environments via the [Concourse Pool Resource](https://github.com/concourse/pool-resource)

* [cf-lts-gcp-environments](cf-lts-gcp-environments) Used to control access to the LTS BOSH-lite environments via the [Concourse Pool Resource](https://github.com/concourse/pool-resource)

* [edge-shared-environments](edge-shared-environments) Used to control access to the CF Deployment environment via the [Concourse Pool Resource](https://github.com/concourse/pool-resource)

* [receipt-diffs](receipt-diffs) Used to determine whether to automatically release a new version of cflinuxfs2

* [binary-verification-whitelist](binary-verification-whitelist) Every day we verify that binaries being distributed via buildpacks.cloudfoundry.org have the correct checksums. Some binaries are, due to development error, known to be wrong. This branch is a list of files to ignore during verification.

* [new-buildpack-cve-notifications](new-cve-notifications) Experimental. Tracks CVEs that affect buildpack dependencies. Currently only implemented for the [ruby-buildpack](https://github.com/cloudfoundry/ruby-buildpack)
