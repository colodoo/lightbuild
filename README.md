# Lightbuild (轻构)

> **Everything is a Component.**  
> **一切皆组件。**

[English](./README.en.md) | 简体中文

Lightbuild（轻构）是一个下一代低代码平台，旨在重新定义应用的构建方式。我们将一切——样式、页面、UI 元素甚至业务逻辑——都视为可组合的组件，从而提供无与伦比的灵活性和开发效率。

---

## 💡 设计理念

**“一切皆组件”** 不仅仅是一句口号，更是我们的核心架构。
- **可视化组件**：标准的 Vue 组件，严格类型化，易于复用。
- **逻辑组件**：封装成可管理单元的业务逻辑。
- **样式组件**：可混合搭配的设计令牌（Tokens）和主题。

## ✨ 核心特性

- **可视化界面构建器**：具备深度定制能力的拖拽式界面。
- **AI 驱动开发**：集成 Spring AI 和 Neo4j，提供基于向量的智能搜索与辅助。
- **流程自动化**：内置 BPMN 引擎，轻松编排复杂工作流。
- **代码级掌控**：嵌入 CodeMirror 编辑器，满足深入细节的开发需求（支持 Java, SQL, JSON, Vue）。
- **数据可视化**：基于 AntV X6 的强大图表能力。

---

## 🛠 技术栈

### 前端 (Frontend)

| 技术 | 说明 |
|------------|-------------|
| **Vue 3** | 渐进式 JavaScript 框架 (Composition API) |
| **Vite** | 下一代前端构建工具 |
| **TypeScript** | 强类型 JavaScript |
| **Element Plus** | 基于 Vue 3 的组件库 |
| **Pinia** | 直观的 Vue.js 状态管理 |
| **AntV X6** | 图可视化引擎 |
| **BPMN.js** | 流程建模工具包 |
| **CodeMirror 6** | 可扩展的代码编辑器 |
| **UnoCSS** | 即时按需原子 CSS 引擎 |

### 后端 (Backend)

| 技术 | 说明 |
|------------|-------------|
| **Java 17** | LTS Java 版本 |
| **Spring Boot 3** | 领先的 Java 应用框架 |
| **MyBatis-Plus** | 强大的 ORM 框架 |
| **Spring AI** | Java AI 应用框架 |
| **Neo4j** | 图数据库与向量存储 |
| **Hutool** | Java 工具类库 |
| **Tika & POI** | 内容分析与办公文档处理 |

### 基础设施 (Infrastructure)

- **Docker & Docker Compose**: 容器化与编排。
- **MySQL 8.0**: 可靠的关系型数据库。
- **Redis 7.0**: 高性能键值存储。
- **Nginx**: 高性能 Web 服务器。

---

## 🚀 快速开始

你可以使用 Docker Compose 快速启动完整技术栈。

### 前置要求

- Docker & Docker Compose
- Java 17+ (用于本地开发)
- Node.js 18+ & pnpm (用于前端开发)

### Docker 启动

```bash
cd docker
docker-compose up -d
```

### 本地开发

**服务端 (Server)**
```bash
cd lightbuild-server
mvn clean install
# 运行 LightbuildServerApplication
```

**前端 (Web)**
```bash
cd lightbuild-web
pnpm install
pnpm dev
```
