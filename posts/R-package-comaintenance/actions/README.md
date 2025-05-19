The GitHub Actions workflows here alert all watchers of a GitHub repository when
the R package hosted in this repo is at risk of archival on CRAN.

The workflows come in two flavours:

- `check-pkg-deadline.yaml` which is meant to be added directly to the repo hosting
the source of the R package. It opens a new issue each time CRAN publishes a deadline before which the package needs to be resubmitted to avoid archival. This allows co-authors to prepare the release even if the listed maintainer is not available. You can see it in action in the [`rmaia/pavo`] repository.
- `check-org-deadlines.yaml` which is meant to be added in any repository of a GitHub organization that also has an R-universe. It will (re)-open a new issue each time one of the packages is at risk of archival. You can see it in action in the [`epiverse-trace/etdashboard`] repository.
