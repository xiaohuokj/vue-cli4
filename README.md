1. npm install -g @vue/cli
   # or
   yarn global add @vue/cli
   查看版本（是否安装成功）：vue -V(大写的V)
2. 命令变化
   Com mands:
   create [options] <app-name>      create a new project powered by vue-cli-service // 创建一个由vue-cli-service支持的新项目
   add <plugin> [pluginOptions]     install a plugin and invoke its generator in an already created project // 在已创建的项目中添加插件
   invoke <plugin> [pluginOptions]  invoke the generator of a plugin in an already created project // 在开发者模式下以零配置运行一个js或vue文件
   inspect [options] [paths...]     inspect the webpack config in a project with vue-cli-service // 在vue-cli-service的项目中检查webpack配置
   serve [options] [entry]          serve a .js or .vue file in development mode with zero config // 简单理解为开发环境下启动命令
   build [options] [entry]          build a .js or .vue file in production mode with zero config // 在生产模式下以零配置构建一个js或vue文件
   init <template> <app-name>       generate a project from a remote template (legacy API, requires @vue/cli-init) // 旧api 需要@vue/cli-init // 就是原来的vue-cli init <template> <app-name>
3. 创建一个项目
   输入以下命令 vue create vue3-cli
   会看到：
   Vue CLI v3.0.0-beta.6
   ? Please pick a preset: (Use arrow keys)
   > xs-default (vue-router, vuex, stylus, babel, pwa, eslint, unit-jest) // 这是我运行过之后的默认设置，第一次执行create是没有的
   default (babel, eslint)
   Manually select features
   按键盘上下键选择默认（default）还是手动（Manually），如果选择default，一路回车执行下去就行了（注：现在vue-cli3.0默认使用yarn下载），这里我选择手动
4. 选择配置，这时你会看见一些选项,
   你要集成什么就选就行了，我这里选个我比较常用的（注：空格键是选中与取消，A键是全选）
   ? Please pick a preset: Manually select features
   ? Check the features needed for your project: (Press <space> to select, <a> to toggle all, <i> to invert selection)
   >( ) TypeScript
    ( ) Progressive Web App (PWA) Support
    ( ) Router
    ( ) Vuex
    ( ) CSS Pre-processors
    ( ) Linter / Formatter
    ( ) Unit Testing
    ( ) E2E Testing
    ? Please pick a preset: Manually select features
    ? Check the features needed for your project: (Press <space> to select, <a> to toggle all, <i> to invert selection)
    >( ) TypeScript
     ( ) Progressive Web App (PWA) Support
     ( ) Router
     ( ) Vuex
     ( ) CSS Pre-processors
     ( ) Linter / Formatter
     ( ) Unit Testing
     ( ) E2E Testing
5. 选择css预处理，这里我选择stylus
6. 选择ESLint + Prettier
7. 选择语法检查方式，这里我选择保存就检测
8. 她会问你 ，把babel,postcss,eslint这些配置文件放哪，这里随便选，我选择放在独立文件夹
    Vue CLI v3.0.0-beta.6
    ? Please pick a preset: Manually select features
    ? Check the features needed for your project: Router, Vuex, CSS Pre-processors, Linter, Unit
    ? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Stylus
    ? Pick a linter / formatter config: Prettier
    ? Pick additional lint features: Lint on save
    ? Pick a unit testing solution: Jest
    ? Where do you prefer placing config for Babel, PostCSS, ESLint, etc.? (Use arrow keys)
    > In dedicated config files // 独立文件放置
      In package.json // 放package.json里
9. 键入N不记录，如果键入Y需要输入保存名字，如第一步所看到的我保存的名字为xs-default
    Vue CLI v3.0.0-beta.6
    ? Please pick a preset: Manually select features
    ? Check the features needed for your project: Router, Vuex, CSS Pre-processors, Linter, Unit
    ? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Stylus
    ? Pick a linter / formatter config: Prettier
    ? Pick additional lint features: Lint on save
    ? Pick a unit testing solution: Jest
    ? Where do you prefer placing config for Babel, PostCSS, ESLint, etc.? In dedicated config files
    ? Save this as a preset for future projects? (Y/n) // 是否记录一下以便下次继续使用这套配置
10. 确定后，等待下载依赖模块
11. 装好后，启动
    cd vue-pro3.0-demo // 进入项目根目录
    yarn serve // 启动项目
12. vue.config需要单独创建，具体看模板里内容（可以自定义配置）

本文网址： https://blog.csdn.net/Alice_124/article/details/81082230


# mycreate

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
