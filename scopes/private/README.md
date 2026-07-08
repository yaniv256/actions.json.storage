# scopes/private/ — placeholder

This is a **placeholder folder**, intentionally empty in the public example. Your private scope holds
owner-only browsing memory, observations, run logs, item indexes, and unreviewed action maps — content
that should never be public.

To use it: create your OWN private git repository and mount it here as a submodule, e.g.

```bash
git submodule add https://github.com/YOUR-ORG/your-actions.json.storage.private.git scopes/private
```

and add a matching `private` mount to `storage.json`. The public example does not link to any private
repo, so nothing here is exposed.
