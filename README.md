优点：
1. 依赖自动提升
2. 交给nx之后，支持开启缓存、内部依赖分析、任务分析
3. 检测改动commit影响的包，区分提示
4. 自带版本控制（能分析出 private:false 的包，引导版本号提升）

缺点：
1. 默认npm, npm@7版本以下不支持monorepo，只能安装根目录的依赖，需要使用lerna bootstrap --hoist，@npm@7版本以上支持，可以直接npm安装所有子包的依赖
