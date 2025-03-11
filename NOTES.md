## Static vs Dynamic rendering

Data rendered **statically** is fetched in _build time_ or when _revalidating data_ (?), which means changes after this point won't be reflected. Helps with SEO and website performance. All non-user specific and general UI data should be rendered statically.

Data rendered **dynamically** is processed at _request time_ - will output the most updated data. Gives us the ability of displaying user-specific content and real time data.

## `useSearchParams()` vs `props.searchParams`

Use the former in client components and the latter in server components.

## Server actions

Run asynchronous code directly on the server through functions that can be invoked from both client and server components.

Behind the scenes, Next creates a POST API endpoint for every server action.

## `error.tsx`

Always a client component. Fallback to all the errors in its folder or child folders. Can be a good place to make error reporting.

## `notFound()` + `not-found.tsx`

`not-found.tsx` will always be displayed by Next when we call `notFound()`. Takes precedence over `error.tsx`

## `next lint`

Warns issues with linting and accessibility - include in the CI/CD pipeline?

## Server-side form validation

Single source of truth when it comes to valid data - no need to validate on both sides.
