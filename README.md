# React Latest (Vite | TypeScript)

This is project generated to serve as a reproduction starter for Storybook.

[View it in Stackblitz](https://stackblitz.com/github/storybookjs/sandboxes/tree/next/react-vite/default-ts/after-storybook?preset=node=)

### Testing instructions

Install dependencies:

```sh
$ yarn
```

Run Storybook:

```sh
$ yarn storybook
```

### What's the problem?

There are two `Button`s for the same component.

![image](https://github.com/abiriadev/sb-csf-plugin-regex/assets/72962900/573d866f-2a17-48a6-949b-7f7a848b00d5)

You can see source [`Button.stories.ts`](src/stories/Button.stories.ts) and [`Button.custom-stories.ts`](src/stories/Button.custom-stories.ts), respectively.

They both have JSDoc comments above each story, but only `Button`'s comments are actually rendered.

https://github.com/abiriadev/sb-csf-plugin-regex/blob/c201a53d791fb9d333376a201f1e993f23e18e7c/src/stories/Button.stories.ts#L26-L29
https://github.com/abiriadev/sb-csf-plugin-regex/blob/c201a53d791fb9d333376a201f1e993f23e18e7c/src/stories/Button.custom-stories.ts#L26-L29

![image](https://github.com/abiriadev/sb-csf-plugin-regex/assets/72962900/e9c71b0c-12aa-4261-9f55-58296493f3ea)

![image](https://github.com/abiriadev/sb-csf-plugin-regex/assets/72962900/494d538f-97fa-49d6-92d9-3482d37e3161)

