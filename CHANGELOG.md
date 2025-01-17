# StarBot_AGLAS 更新日志 Changelog

## [v2.0.1 Beta 0.95]-图片生成方案优化&QQ频道兼容

- 修复今日运势图片生成过程中推分率数字不居中的问题，提升生成图片的美观度（居中误差已降低到2px内）
  > ⚠️给魔改玩家的提示：此更新中对误差分析、图片生成过程使用的锚定对齐参数（anchor）仅限TrueType字体可用，若您需要更换本图片生成方案中的HOS.ttf为非TrueType字体，请自行重新调节字体对齐方法及起始坐标参数
- 更换b40/b50中使用的部分字体，提升美观度
- 移除本地QQ频道兼容插件，改用[nonebot-plugin-guild-patch](https://github.com/mnixry/nonebot-plugin-guild-patch)，并同步更新`requirements.txt`以及`plugin-list.json`，完成了所有本地插件对QQ频道的兼容

## [v2.0.1 Beta 0.93]-自KibaBot重制&修复

- 自KibaBot 5.0.1开始重制
- 移除比大小游戏玩法
- 修复b40/b50牌子、称号数据库问题
- 开始适配Python 3.10 及 Onebot v11协议（未适配完成的插件位于`src\Construct`文件夹内）
- 修复b40/b50找不到字体、图片的问题
- Arcaea及coc模块自机器人分离，使用nonebot插件商店内的项目并保持更新
  - Arcaea模块使用[nonebot-plugin-arcaeabot](https://github.com/SEAFHMC/nonebot-plugin-arcaeabot)
  - coc模块使用[nonebot_plugin_cocdicer](https://github.com/abrahum/nonebot_plugin_cocdicer)
- 修改插件加载方式，使StarBot可以同时加载`plugin-list.json`内列出的商店插件和本体自带模块
- 修复`database.py`中漂流社区的数据表存在错误字段的问题
- 更新依赖并修复若干依赖版本冲突
- 修复可能发生的`Max retries exceeded with url`错误
- 若干功能修复
