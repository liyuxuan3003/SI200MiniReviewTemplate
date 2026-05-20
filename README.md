# SI200MiniReviewTemplate

SI200MiniReviewTemplate是一个开箱即用的LaTeX模板，适用于上海科技大学SI200课程小综述，基于自定义文档类`si200-mini-review`。

SI200MiniReviewTemplate是LumosLaTeX计划的一部分：https://github.com/liyuxuan3003/LumosLaTeX

https://github.com/liyuxuan3003/SI200MiniReviewTemplate.git

## 引入方式

克隆模板仓库

```bash
git clone git@github.com/liyuxuan3003/SI200MiniReviewTemplate.git
```

初始化项目

```
cd SI200MiniReviewTemplate
./init.sh MyProject
```

初始化会自动完成项目重命名、子模块加载、移除模板的远程引用等操作，只能执行一次。

## 目录结构

项目的目录结构如下

```
SI200MiniReviewTemplate # The root of git repo
|- .git
|- MyProject            # The sub dir of source files (run make here!)
.  |- build/
.  |- makefile-latex/
.  |- minimus/
.  |- si200-mini-review/
.  |- Makefile
.  |- MyProject.tex
|- .gitignore
|- .gitmodules
|- init.sh
|- README.md
|- SI200MiniReview.md
```

请注意，根目录下仅有`.gitignore`和`README.md`等文件，代码均位于一个二级目录下！

## 构建方式

模板提供`Makefile`进行编译，任何`make`命令都需要在二级目录下运行。

编译文档及其插图

```bash
make -j
```

清理文档输出目录

```bash
make clean
```

## 子模块

模板的具体使用方式，请参见各个子模块的文档。

| 子模块 | 文档 |
|--------|------|
| `minimus` | [README](SI200MiniReview/minimus/README.md) |
| `si200-mini-review` | [README](SI200MiniReview/si200-mini-review/README.md) |
| `makefile-latex` | [README](SI200MiniReview/makefile-latex/README.md) |
