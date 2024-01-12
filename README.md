# 项目搭建
## 创建项目
```js
pnpm create vue@latest app-name
```
更新依赖包到最新版本
```js
pnpm up --latest
```
## 安装插件
### vue devtools集成
```js
pnpm add -D vite-plugin-vue-devtools@latest
```
修改vite.config.js文件
```js
export default defineConfig({
  plugins: [vue(), vueJsx(), VueDevTools(options)],
  resolve: {
    alias: {
      '@': fileURLToPath(new URL('./src', import.meta.url))
    }
  }
})
```
### UI组件库的引入
```js
```