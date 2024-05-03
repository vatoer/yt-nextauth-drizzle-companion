sebelum lanjut buat setting untuk editor VS code

```json
{

  "editor.formatOnPaste": true,

  "editor.formatOnSave": true,

  "editor.indentSize": "tabSize",

  "editor.tabSize": 2,

  "editor.wordWrap": "wordWrapColumn",

  "editor.wordWrapColumn": 120,

  "editor.codeActionsOnSave": {

    "source.fixAll.eslint": "explicit",

    "source.sortImports": "explicit"

  },

  "files.eol": "\n"

}
```

<https://nextjs.org/docs/app/building-your-application/routing/route-groups>

<https://authjs.dev/getting-started/authentication/oauth>

membuat group `(auth)` yang akan berisi `login` dan `register` serta komponennya

```tree
-src\app\(auth)\
	- _components
	- login
		- _components
		- page.tsx
	- register
		- _components
		- page.tsx
```

membuat alias `src\app\(auth)\` menjadi `@/app/auth/` di `tsconfig.json` 

```json
"paths": {

      "@/*": ["./src/*"],

      "@/app/auth/*": ["./src/app/(auth)/*"]

    }
```
## Install shadcn

<https://ui.shadcn.com/docs/installation/next>
<https://ui.shadcn.com/docs/components/button>

```sh
pnpm dlx shadcn-ui@latest add button
```

## Add react-icons

```sh
pnpm add react-icons
```

Add layout to auth `src/app/(auth)/layout.tsx`

## handle Login with google

add function to `LoginWithGoogle` component

## handle Login with credentials

<https://react-hook-form.com/get-started/>

```sh

pnpm add react-hook-form

```

  

<https://zod.dev/?id=from-npm-nodebun>

  

```sh

pnpm add zod @hookform/resolvers

```

update `auth.ts`
