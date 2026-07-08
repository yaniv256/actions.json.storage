# actions.json.storage (example structure)

A public **example** of the `actions.json.storage` root/index workspace: it records storage
configuration, mounted scope repositories, and layout. It is not a place for raw browsing
observations or private overlays — those belong in your own private scope.

## Layout

```text
storage.json     Root storage manifest (mounts, visibility, sync policy)
.gitmodules      Mounted scope repositories
scopes/
  public/        Submodule: reviewed, reusable public site maps
  private/       (your own private repo — wire it yourself; not included here)
```

## Using this as a template
Fork or copy this structure, point `scopes/private` at your OWN private repo in `storage.json`
and `.gitmodules`, and keep only the `public` scope shared. Add further scopes as separate
repositories as needed.
