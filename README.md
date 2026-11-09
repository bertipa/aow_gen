# aow_gen — mailbox for the aow-gen worker

Jobs go in `queue/` (one TOML file each, run in file-name order); the worker
on aiserv writes `results/<job id>/` (`status.toml` plus sheets, previews or
pick sidecars) and pushes. The worker, the job types and the trust model are
documented in aow_sphere `tools/gen/README.md`.

This repository holds data only: the worker's code comes from aow_sphere
`main`, never from here.
