# Verve

Verve 是一个用 Vix 编写的代码格式化工具，用于自动格式化 `.vix` 文件，统一缩进和空行风格。

## 使用方式

### 直接执行（推荐）

```bash
very exe verve
```

`very exe verve` 会自动构建并运行 Verve。Verve 会递归扫描当前目录下所有 `.vix` 文件，自动修正缩进并合并多余空行。

### 仅构建

```bash
very build
```

`very build` 会读取 `vindex.toml` 配置，编译 `main.vix` 及 `src/` 下的源文件，生成可执行文件。一般不需要单独执行，`very exe` 会自动处理构建。

## 项目说明

- `main.vix` — 入口文件，实现文件扫描与格式化逻辑
- `src/lib.vix` — 库模块
- `vindex.toml` — 项目配置
