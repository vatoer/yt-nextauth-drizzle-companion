<https://authjs.dev/getting-started/installation>


**Configuration File**: Show how to create a NextAuth configuration file (usually `auth.config.js` or `auth.js`) where you'll define your authentication providers and other options.

```sh

openssl rand -hex 32

```

Then add it to your `./.env.local` file:

create `src/auth.ts`

```ts
import NextAuth from "next-auth"
 
export const { handlers, signIn, signOut, auth } = NextAuth({
  providers: [],
})
```

create `src/middleware.ts`

```ts

export { auth as middleware } from "@/auth"

```

**Authentication Providers**: Explain the concept of authentication providers supported by NextAuth (e.g., email/password, Google, Facebook, GitHub) and discuss which providers will be used in the tutorial.

[Penyedia Otentikasi](03-a1-Penyedia Otentikasi.md)

**Setting up OAuth Providers**: If using OAuth providers like Google, Facebook, or GitHub, demonstrate how to obtain client IDs and secrets and configure them in the NextAuth configuration file.

[OAuth Google](03-a2-Oauth google.md)

update `./.env.local`

```.env
AUTH_GOOGLE_ID={AUTH_GOOGLE_ID}

AUTH_GOOGLE_SECRET={AUTH_GOOGLE_SECRET}
```

update `@/auth`

```ts
-providers: [],
+providers: [Google],
```

**Custom Callbacks and Redirects**: Explain how to define custom callback URLs and redirects for different authentication flows, such as login, logout, and error handling.

**Session Management**: Discuss NextAuth's built-in session management and how sessions are managed and persisted across requests.

