[![Update Fancyss Rules](https://github.com/waitusz/fancyss-rules/actions/workflows/fancyss-rules-3.0.yml/badge.svg)](https://github.com/waitusz/fancyss-rules/actions/workflows/fancyss-rules-3.0.yml)
[![](https://data.jsdelivr.com/v1/package/gh/waitusz/fancyss-rules/badge?style=rounded)](https://www.jsdelivr.com/package/gh/waitusz/fancyss-rules)

#### Update 2022/9/24: 支持了[3.0](https://github.com/hq450/fancyss)版本，旧版本规则将在[这里](https://github.com/waitusz/fancyss-rules/tree/master)保留并继续更新
---   
#### 每日UTC+8 3:45时自动更新规则，推荐在插件中设置每天4:00定时更新  
---
### 食用方法：
- 进入路由器SSH，运行以下命令会自动将`ss_rule_update`脚本中的`url_main`参数指向我的仓库（二选一即可）：
- `sed -i 's/^URL_MAIN.*/URL_MAIN="https:\/\/raw.githubusercontent.com\/waitusz\/fancyss-rules\/3.0\/rules"/g' /koolshare/scripts/ss_rule_update.sh`  （**推荐**，直连GitHub仓库）
- `sed -i 's/^URL_MAIN.*/URL_MAIN="https:\/\/cdn.jsdelivr.net\/gh\/waitusz\/fancyss-rules@3.0\/rules"/g' /koolshare/scripts/ss_rule_update.sh`  （仅当更新规则时显示`"没有检测到在线版本。可能是访问github有问题"`时推荐，由于jsDelivr CDN存在最长24小时的缓存，规则更新会有延迟）
- > x86版本fancyss插件请自行找到更新规则的脚本并替换`url_main`参数
### 每次fancyss插件更新后都需要\*重新运行一次\*更新`ss_rule_update`脚本的命令
