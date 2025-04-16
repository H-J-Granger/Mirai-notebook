# Mirai-notebook
未来的笔记，主要关于数学、物理与理论计算机科学。  
Mirai's notebook, mainly in math, physics, and theoretical computer science.

---

笔记的框架主要参考中国科学技术大学少年班学院的数学与应用数学专业及物理学专业的 [培养方案](https://www.teach.ustc.edu.cn/education/241.html)。

## 如何编译

我会建议使用 Ubuntu 22.04 上的 TeXLive 2022，利用如下版本编译。没有测试在其他版本下能否正常运行。
```bash
cd <想要编译的文件所在目录，譬如 分析学/1-数学分析>
latexmk -synctex=1 -interaction=nonstopmode -file-line-error -xelatex -outdir=. main.tex
bibtex main
latexmk -synctex=1 -interaction=nonstopmode -file-line-error -xelatex -outdir=. main.tex
latexmk -synctex=1 -interaction=nonstopmode -file-line-error -xelatex -outdir=. main.tex
```

## License

本人对笔记内容的原创性（几乎）没有贡献。笔记内的引用均遵循学术界惯例，对此笔记的引用也还请同样循惯例。