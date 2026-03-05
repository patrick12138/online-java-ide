# 在线 Java IDE（Spring Boot）

[English](./README.md) | [简体中文](./README.zh-CN.md)

一个基于 Spring Boot 的轻量级在线 Java IDE。它可以执行浏览器提交的 Java 源码中的 `main` 方法，并将标准输出和运行时异常信息返回到页面。

## 功能特性

- 在网页中编译并运行 Java 源码。
- 支持捕获并展示：
  - 标准输出（`System.out`），
  - 运行时异常信息，
  - 标准输入（`System.in`）内容。
- 内置执行时长限制，降低长时间运行任务的风险。

## 技术栈

- Java 8
- Spring Boot 2.7
- Thymeleaf
- Maven

## 快速开始

### 1）环境要求

- JDK 8+
- Maven 3.6+

### 2）运行项目

```bash
mvn spring-boot:run
```

### 3）浏览器访问

访问：<http://localhost:8080>

## 使用方式

1. 打开首页。
2. 输入 Java 代码（需包含 `public static void main(String[] args)`）。
3. （可选）填写标准输入内容。
4. 点击运行并查看输出结果。

## 项目结构

```text
src/main/java/com/patrick/onlineide
├── compile      # 源码编译
├── controller   # Web 入口与页面路由
├── execute      # 运行执行 / IO 重定向 / 类加载
└── service      # 应用服务层
```

## 许可证

当前仓库未包含独立的许可证文件。如果你计划公开开源，建议补充 License。
