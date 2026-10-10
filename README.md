# Encrypted processing handoff

This branch contains only the latest age-encrypted ZIP batch and its version 2 manifest.
The absence of batch.json means no current work. Read the manifest and artifact from one commit.
Do not scan history or other references. Discard pending work downloaded before this reset epoch.
Keep prior completion history; deduplicate by batchId and ZIP file number, never by node id.
The ZIP contains 1.json, 2.json, ... with {id: node UUID, account: Native export object}.
Only Sidecar writes this branch after initialization. The consumer retains its private age identity.
