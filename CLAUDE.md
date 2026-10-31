# CLAUDE.md - 天气预报插件 (weather-forecast) (whitefox_weather-forecast)

## 1. 模块定位与系统职责
- **插件标识符**：`whitefox_weather-forecast`
- **当前生效版本**：`v2.0.1`
- **托管仓库**：[`Wenaixi/weather-forecast`](https://github.com/Wenaixi/weather-forecast)
- **核心定位**：高德地图天气预报：早晚定时群播报与手动查询天气。

## 2. 关键工程规范与配置说明
- **配置路径**：`config.toml`（所有业务调优与鉴权参数收敛于此）；
- **数据持久化**：优先遵循 MaiBot SDK 标准持久化规范，不直接向源码目录写入易失数据；
- **编码与日志规范**：严格遵循 PEP 8 风格，文档与代码注释杜绝 emoji，避免虚假套话。

## 3. 本地深度定制与稳定性修复
导出通用天气查询 API (plugin.weather.get_current_weather)，修复 API 装饰器导入，为麦迹日记提供实时的福清地理天气与温度。

---

## 上游项目与开源溯源
- **原作者 / 组织**：`whitefox`
- **官方上游仓库**：[https://github.com/whitefox/weather-forecast](https://github.com/whitefox/weather-forecast)
- **开源许可证**：`MIT`
- **分支演进模式**：本仓库作为主人的深度定制与生产维护分支（`Wenaixi/weather-forecast`）。在保持与官方上游架构演进对齐的同时，锁死并持续维护针对本服务器生产环境的稳定性补丁与核心特性。
