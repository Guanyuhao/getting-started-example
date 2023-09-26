# Lerna Getting Started Example

- jest 配置支持 Monorepo
- 轻量Monorepo Lerna + pnpm + workspace
- 增加 git-validator

```
pnpm install 
lerna run build
lerna run test 
```

## 构建是否缓存测试
```
lerna run build --scope=header
```

This repo is a small example of using Lerna 5+.

Watch this [10-minute walkthrough](https://youtu.be/1oxFYphTS4Y) to see how new versions of Lerna work.

> Note: The video was recorded with Lerna 6. Some information within it may be outdated. See [the Getting Started docs](https://lerna.js.org/docs/getting-started#adding-lerna-to-an-existing-repo) for up-to-date instructions for the latest version of Lerna.

This repo contains three packages or projects:

- `header` (a library of React components)
- `footer` (a library of React components)
- `remixapp` (an app written using the Remix framework which depends on both `header` and `footer`)

```
packages/
    header/
        src/
            ...
        package.json
        rollup.config.json
        jest.config.js

    footer/
        src/
            ...
        package.json
        rollup.config.json
        jest.config.js

    remixapp/
        app/
            ...
        public/
        package.json
        remix.config.js

package.json
```
