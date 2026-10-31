# 天气预报插件 (weather-forecast)

> 本插件由 [Wenaixi](https://github.com/Wenaixi) 维护，是专为生产环境深度调优的高可用分支。

## 简介与定位

高德地图天气预报：早晚定时群播报与手动查询天气。

- **插件目录**：`whitefox_weather-forecast`
- **生效版本**：`v2.0.1`
- **开源许可证**：`MIT`

---

## 核心特性与本地深度调优

- 导出通用天气查询 API (plugin.weather.get_current_weather)，修复 API 导入，为麦迹日记提供实时的福清地理天气与温度

---

## 指令与工具速查

### 常用指令 (Command)
- `/天气 <城市> - 手动查询指定地点天气预报`

### 大模型工具 (Tool)
- `@Tool("weather_query") - 查询城市气象预报工具`

---

## 快速配置

配置文件统一定位于插件根目录下的 `config.toml`。修改后重启或通过 WebUI 热重载即可生效。

---

## 上游项目与开源溯源

- **原作者 / 组织**：`whitefox`
- **官方原版开源仓库**：[https://github.com/whitefox/weather-forecast](https://github.com/whitefox/weather-forecast)
- **开源协议**：`MIT`
- **声明**：本项目遵循开源协议，特此致敬原作者的杰出贡献。本分支针对生产环境的高并发网络、个性化社交和抗风控需求进行了深度稳定性修复与定制化演进。
