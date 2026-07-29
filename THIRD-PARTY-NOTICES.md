# 第三方组件许可清单（Third-Party Notices）

同堂 Tongtang 的发行镜像（`jeesa/tongtang`、`jeesa/tongtang-web`、`jeesa/tongtang-api`、`jeesa/tongtang-mt`）包含以下第三方开源组件。各组件版权归其原作者所有，依其原始许可分发；本清单随发行一并提供以履行署名义务。

## 后端（jeesa/tongtang-api · jeesa/tongtang）

| 组件 | 版本 | 许可 | 项目 |
|---|---|---|---|
| FastAPI | 0.115.14 | MIT | https://github.com/fastapi/fastapi |
| Uvicorn | 0.34.3 | BSD-3-Clause | https://github.com/encode/uvicorn |
| httpx | 0.28.1 | BSD-3-Clause | https://github.com/encode/httpx |
| Pydantic | 2.11.7 | MIT | https://github.com/pydantic/pydantic |
| websockets | 15.0.1 | BSD-3-Clause | https://github.com/python-websockets/websockets |
| python-multipart | 0.0.20 | Apache-2.0 | https://github.com/Kludex/python-multipart |
| aiomqtt | 2.3.0 | BSD-3-Clause | https://github.com/empicano/aiomqtt |
| paho-mqtt（aiomqtt 依赖） | 2.x | EPL-2.0 / EDL-1.0 双许可（按 EDL-1.0 采用） | https://github.com/eclipse-paho/paho.mqtt.python |
| segno | 1.6.6 | BSD-3-Clause | https://github.com/heuer/segno |
| HAP-python | 4.9.2 | Apache-2.0 | https://github.com/ikalchev/HAP-python |
| base36（HAP-python[QRCode] 附带） | 0.x | MIT | https://github.com/tonyseek/python-base36 |
| Python 运行时 | 3.12 | PSF-2.0 | https://www.python.org |

## 前端（jeesa/tongtang-web · jeesa/tongtang）

| 组件 | 版本 | 许可 | 项目 |
|---|---|---|---|
| React / React DOM | 19.2.0 | MIT | https://github.com/facebook/react |
| Material Design Icons（@mdi/js） | 7.4.47 | Apache-2.0 | https://github.com/Templarian/MaterialDesign-JS |
| Phosphor Icons（@phosphor-icons/react） | 2.1.10 | MIT | https://github.com/phosphor-icons/react |
| Vite / @vitejs/plugin-react（构建工具） | 6.4.2 | MIT | https://github.com/vitejs/vite |
| nginx（web 镜像基座） | stable | BSD-2-Clause | https://nginx.org |

## Matter 侧车（jeesa/tongtang-mt）

| 组件 | 版本 | 许可 | 项目 |
|---|---|---|---|
| matter.js（@matter/main） | 0.16.11 | Apache-2.0 | https://github.com/project-chip/matter.js |
| ws | 8.x | MIT | https://github.com/websockets/ws |
| Node.js 运行时 | 20 | MIT（自带第三方清单见其发行） | https://nodejs.org |

## 其他说明

- 各容器基础镜像（Debian slim / nginx 官方镜像等）内的操作系统组件依其各自许可分发，完整清单见对应基础镜像的发行说明。
- 同堂经 REST / WebSocket API 与 Home Assistant（Apache-2.0）交互，不包含、不分发其代码。
- 开发期用于设备词汇核对的 zigbee-herdsman-converters（GPL-3.0）仅作离线比对，无任何代码或数据进入发行产物。
- 上述 MIT / BSD-2-Clause / BSD-3-Clause / Apache-2.0 / EDL-1.0 / PSF-2.0 许可全文见各项目仓库或 https://opensource.org/licenses 。所有 Apache-2.0 组件均未经修改直接使用。
