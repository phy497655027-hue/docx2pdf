# PDF转Word转换器

一个简单易用的PDF转Word转换工具，基于WPF开发，支持批量转换和自定义输出路径。

## 功能特点

- 将PDF文件转换为Word文档
- 支持批量转换多个PDF文件
- 自定义输出路径
- 简洁直观的用户界面
- 实时显示转换进度

## 系统要求

- Windows 10 或更高版本
- .NET 10.0 Windows 运行时

## 安装与运行

### 从源代码运行

1. 克隆或下载此项目到本地
2. 使用Visual Studio或.NET CLI打开项目
3. 恢复依赖包并运行项目

```bash
# 使用.NET CLI
cd PdfWordConverter
dotnet restore
dotnet build
dotnet run
```

### 使用发布版本

1. 从发布版本下载最新的可执行文件
2. 解压到任意文件夹
3. 双击运行PdfWordConverter.exe

## 使用说明

1. 启动程序后，点击"选择PDF文件"按钮选择要转换的PDF文件
2. 选择输出路径（可选，默认为原PDF文件所在目录）
3. 点击"开始转换"按钮开始转换
4. 等待转换完成，转换后的Word文件将保存在指定路径

## 项目结构

```
PdfWordConverter/
├── Resources/           # 资源文件（图标等）
├── MainWindow.xaml     # 主窗口界面定义
├── MainWindow.xaml.cs   # 主窗口逻辑
├── ProgressWindow.xaml # 进度窗口界面定义
├── ProgressWindow.xaml.cs # 进度窗口逻辑
└── PdfWordConverter.csproj # 项目文件
```

## 开发

### 构建项目

```bash
dotnet build
```

### 发布项目

```bash
# 发布为依赖框架的版本
dotnet publish -c Release -r win-x64 --self-contained false

# 发布为独立版本
dotnet publish -c Release -r win-x64 --self-contained true
```

## 许可证

本项目仅供学习和个人使用。

## 贡献

欢迎提交问题报告和改进建议。
