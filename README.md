# Database
# Linux 数据库一键部署脚本 database.sh

🚀 Linux 生产级环境 | Redis + PostgreSQL + MySQL 三合一 | TUI 中文可视化界面 | 自定义目录 | 集群支持 | 内核自动优化

---

# 支持的Linux系统
1.0,2.0用APT包管理器
3.0级以上支持所有Linux包管理器

## 项目介绍
这是一款专为 Linux 服务器打造的数据库全自动部署脚本，
保留极简流畅的 TUI 交互，支持三大主流数据库，一键完成安装、配置、优化、开机自启、集群配置。

适合：
• 新手快速搭建数据库
• 开发者/学生搭建项目环境
• 运维人员批量部署
• 个人服务器/云服务器使用

---

## 支持数据库
• 🐘 PostgreSQL
• 🐬 MySQL
• Redis

## 为什么选择这三大数据库？
本脚本旨在覆盖**99% 的服务器运维场景**，以下是对三大主流数据库的特性解析：

### 🔴 Redis：性能霸主
*   **核心优势**：**极速响应**（毫秒级）、高并发承载能力极强。
*   **适合**：作为项目的**缓存层**加速查询，或者作为**消息队列**处理异步任务。你的脚本已优化内核参数，专为高并发连接而生。

### 🔵 PostgreSQL：全能王者
*   **核心优势**：**数据完整性**与**复杂查询**能力天花板。如果你需要存储复杂的 JSON 结构、进行复杂的统计分析或要求数据绝对安全，PostgreSQL 是首选。
*   **适合**：核心业务系统、金融级数据、需要强事务一致性的场景。

### 🟡 MySQL：普及标准
*   **核心优势**：**生态成熟**、部署简单、社区活跃。对于绝大多数 Web 应用（如 Laravel、Spring Boot），MySQL 仍是开箱即用的最佳选择。
*   **适合**：通用型业务、博客、论坛、中小型企业内部系统。

---

### 📊 场景选型指南
| 业务场景 | 推荐数据库 | 理由 |
| :--- | :--- | :--- |
| **接口缓存 / 热点数据** | **Redis** | 内存读写，极致速度 |
| **电商交易 / 账务系统** | **PostgreSQL** | 强大的事务控制，数据防篡改 |
| **个人博客 / 小型网站** | **MySQL** | 稳定易用，生态普及 |
| **社交/Feed 流/排行榜** | **Redis + PostgreSQL** | Redis 做实时计数，PG 做持久化存储 |

---

## 核心功能
• 中文 TUI 可视化操作
• 自定义安装目录，不写死路径
• 自动优化内核参数（高并发必备）
• 密码隐藏输入 * 号显示
• 端口自定义
• 监听 IP 自定义
• 数据库集群开关 + 节点数量选择
• systemd 托管，开机自启
• 统一管理命令：start / stop / restart / status

---

## 使用方法
1. 下载脚本
下载命令:(如有curl)
1.0.0:
curl -L https://github.com/du-zihan/Database/releases/download/v1.0.0/Database.sh | bash

2.0.0:
curl -L https://github.com/du-zihan/Database/releases/download/v2.0.0/Database.sh | bash

3.0.0:
curl -L https://github.com/du-zihan/Database/releases/download/v3.0.0/Database.sh | bash

3. 按界面提示完成部署

部署后管理：
./database.sh redis start
./database.sh postgres stop
./database.sh mysql restart

---

## 支持系统
Ubuntu / Debian / CentOS / Rocky / AlmaLinux / Fedora / Alpine 等主流 Linux 发行版

---

## 版权声明
本项目遵循 GPL-3.0开源协议，可自由使用、修改、分发，禁止闭源商用。
许可证内容:https://www.gnu.org/licenses/gpl-3.0.html

---

## 免责声明
本脚本仅供学习与测试使用，部署线上环境请自行评估风险。
作者不对数据丢失、服务器故障、安全问题承担责任。

---

## 反馈
欢迎反馈!
本脚本如有不足，请留下你的lssues
开发者邮箱:duzihan111@163.com

---

如果你觉得本仓库对你有用，请留个star⭐
求求了∽🙏
