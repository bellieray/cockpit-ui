# cockpit-ui

Static shell for a private analytics panel. It holds no data and no credentials:
every number is fetched at runtime from a private endpoint that requires a
read-only key the viewer supplies themselves.

Published here because the API host (Supabase Edge Functions) rewrites
`text/html` to `text/plain` on its free plan, so the page cannot be served
from the same origin as the data.

Source of truth: the `web/` directory of the private `app-cockpit` repository.
