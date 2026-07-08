# actions.json.storage (example structure)

A public **example** of the `actions.json.storage` root/index workspace: it records storage
configuration, mounted scope repositories, and layout. It is not a place for raw browsing
observations or private overlays — those belong in your own private scope.

## ⚠️ Privacy — you must enforce it

This example is public. If you fork or copy it and start storing your OWN data, **nothing here makes
your private data private automatically.** You must enforce privacy in one of two ways:

1. **Keep your whole fork private** — after forking, set the repository visibility to Private. Then
   everything, including `scopes/private`, stays private.
2. **Make `scopes/private` a submodule pointing at your OWN private repo** — keep this root repo
   public if you like, but mount the private scope from a separate **private** repository. Your private
   content then lives in that private repo, never in the public root.

If you do neither and push private content into a public fork, it will be exposed. See
`scopes/private/README.md`.

## Layout

```text
storage.json     Root storage manifest (mounts, visibility, sync policy)
.gitmodules      Mounted scope repositories
scopes/
  public/        Submodule: reviewed, reusable public site maps
  private/       Placeholder — mount your OWN private repo here (see its README)
```

## Using this as a template
Fork or copy this structure, decide your privacy model (above), point `scopes/private` at your OWN
private repo in `storage.json` and `.gitmodules` if using option 2, and keep only the `public` scope
shared. Add further scopes as separate repositories as needed.
