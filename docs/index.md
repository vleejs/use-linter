Prettier 是一个固执己见的代码格式化程序

- [jsx](https://facebook.github.io/jsx/#sec-rationale)
- [ang](https://angular.io/)
- [less](https://lesscss.org/)
- [sass](https://sass-lang.com/)
- [yaml](https://yaml.org/)

## Prettier vs linter

- prettier 格式化：解决代码格式问题
- linter 捕获错误：解决代码质量问题

```sh
pnpm add --save-dev --save-exact prettier

pnpm exec prettier . --write

## 格式化某个目录
pnpm exec prettier --write docs/

npx prettier . --check

## 排除某些文件不添加到 .prettierignore
prettier . "!**/*.{js,jsx,vue}" --write
```

```js
// old
function foo() {}
foo(1, 0, 0, 0, 1, 0, 0, 0, 1)

// new
function foo() {}
foo(1, 0, 0, 0, 1, 0, 0, 0, 1)
```

```sh
npx mrm@2 lint-staged
```

## CLI

```sh
# 格式化所有的
npx prettier . --write

# 检查所有的
npx  prettier . --check
```

## options

```
语句末尾的分号
semi: true,

export default {
  printWidth: 80,
  tabWidth: 2, // 缩进级别的空格数
  useTabs: false, // default
  semi: true,
};

semi: false,

```

## 扩展

- [社区的插件](https://prettier.io/docs/en/plugins#community-plugins)
