[![GitHub release](https://img.shields.io/badge/release-1.0.0-28a745.svg)](https://github.com/0nebean/com.alibaba.druid-0nebean.custom/releases)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)


Introduction
---
- The secondary development druid dataSource connection pool
- has been added to allow you to perform drop function,create function
- 二次开发的 druid 数据库连接池
- 允许执行 drop function,create function等操作



Documentation
---
- config
```
        ......
        WallConfig wallConfig = new WallConfig();
        
        /*add the following line config*/
        /*添加下面这行配置*/
        wallConfig.setCreateFunctionAllow(true);
        wallConfig.setSetAllow(true);
        
        
        
        WallFilter wallFilter = new WallFilter();
        wallFilter.setConfig(wallConfig);
        List<Filter> filters = new ArrayList<>();
        filters.add(wallFilter);
        datasource.setProxyFilters(filters);
        ......
```
---
# [com.alibaba.druid](https://github.com/alibaba/druid.git)

