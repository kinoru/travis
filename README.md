This is an empty repository that serves as an upload endpoint. Travis CI will upload its releases here, and they will be harvested manually.

## Why do I need this?

- Travis CI can't upload a GitHub release as a _release draft_. You can't review your release before you publish it. Mind you, once you publish a release, it's official, and people may accidentally download it, even when it's not quite verified by the repository owner.
- When there are two or more platforms defined in the Travis matrix, Travis CI can't distinguish them correctly while processing the "deploy" field. You can't upload multiple release assets (for different platforms) to a same GitHub release.
