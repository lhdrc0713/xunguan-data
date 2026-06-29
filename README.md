# 今日寻观远程数据

这个目录用于托管国家宗教事务局宗教活动场所数据，适合上传到 GitHub Pages、对象存储或自己的 HTTPS 服务器。

- `data/manifest.json`：总索引，包含宗教/派别统计和城市数据文件列表。
- `data/cities/*.json`：按省市拆分的场所数据，行字段顺序见每个文件的 `fields`。

小程序不要直接打包这个目录；正式环境通过 `wx.request` 按城市加载对应 JSON。
