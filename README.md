# Online Java IDE (Spring Boot)

[English](./README.md) | [简体中文](./README.zh-CN.md)

A lightweight online Java IDE built with Spring Boot. It can execute the `main` method of Java source code submitted from the browser, then return standard output and runtime exception information to the page.

## Features

- Compile and run Java source code entered in the web page.
- Capture and display:
  - standard output (`System.out`),
  - runtime exceptions,
  - program input (`System.in`) support.
- Built-in execution time limit to reduce long-running task risk.

## Tech Stack

- Java 8
- Spring Boot 2.7
- Thymeleaf
- Maven

## Quick Start

### 1) Prerequisites

- JDK 8+
- Maven 3.6+

### 2) Run

```bash
mvn spring-boot:run
```

### 3) Open in browser

Visit: <http://localhost:8080>

## Usage

1. Open the home page.
2. Enter Java code (a class that includes `public static void main(String[] args)`).
3. (Optional) Provide standard input text.
4. Click run to execute and view output.

## Project Structure

```text
src/main/java/com/patrick/onlineide
├── compile      # Source compilation
├── controller   # Web endpoints and page routing
├── execute      # Runtime execution / IO redirection / class loading
└── service      # Application service layer
```

## License

This project currently does not include a dedicated license file. Add one if you plan to open-source it publicly.
