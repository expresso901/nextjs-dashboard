## Next.js App Router Course - Starter
This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.
For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

So's note:
Adding font, clsx, conditioning styling
<Link> allows you to do client-side navigation with JavaScript, while <a> refresh page
confirm github is working. 
Chapter 7 fetching data
Only 1 database could be created and the database is share with the nextjs project.
Dynamic rendering using no store in chapter 8
Streaming is a data transfer technique that allows you to break down a route into smaller "chunks" and progressively stream them from the server to the client as they become ready.
loading.tsx is a special Next.js file built on top of Suspense, it allows you to create fallback UI to show as a replacement while page content loads.
Straming by using suspense.
const searchParams = useSearchParams();
const pathname = usePathname();
const { replace } = useRouter();
const params = new URLSearchParams(searchParams); 
params.set('query', term);
replace(`${pathname}?${params.toString()}`);
URLSearchParams is a Web API that provides utility methods for manipulating the URL query parameters. Instead of creating a complex string literal, you can use it to get the params string like ?page=1&query=a.
<Search> is a Client Component, so you used the useSearchParams() hook to access the params from the client.
<Table> is a Server Component that fetches its own data, so you can pass the searchParams prop from the page to the component.
import { useDebouncedCallback } from 'use-debounce';
Complete chapter 12 with zod and form data handling
Complete chapter 13 with error and not-found
Complete chapter 14 by useFormState to validate and display error
Compeleted chapter 15 authenication...have to update env in deployment]
completed chapterb 16 metadata and all.