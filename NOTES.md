## Static vs Dynamic rendering

Data rendered **statically** is fetched in _build time_ or when _revalidating data_ (?), which means changes after this point won't be reflected. Helps with SEO and website performance. All non-user specific and general UI data should be rendered statically.

Data rendered **dynamically** is processed at _request time_ - will output the most updated data. Gives us the ability of displaying user-specific content and real time data.

## `useSearchParams()` vs `props.searchParams`

Use the former in client components and the latter in server components.
