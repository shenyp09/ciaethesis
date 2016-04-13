# What's CiaeThesis?
CiaeThesis is a LaTeX thesis template package for China Institute of Atomic Energy supporting master, doctor dissertations. Since the users of this package are supposed to be Chinese or those understand Chinese, the following of this file and all other documents are written in Chinese only.

# Makefile的用法

```shell
make [{all|thesis|shuji|doc|clean|cleanall|distclean}] \
     [METHOD={latexmk|xelatex|pdflatex}]
```

## 目标
* `make all`       等于 `make thesis && make shuji && make doc`；
* `make cls`       生成模板文件；
* `make thesis`    生成论文 main.pdf；
* `make shuji`     生成书脊 shuji.pdf；
* `make doc`       生成使用说明书 thuthesis.pdf；
* `make clean`     删除示例文件的中间文件（不含 main.pdf）；
* `make cleanall`  删除示例文件的中间文件和 main.pdf；
* `make distclean` 删除示例文件和模板的所有中间文件和 PDF。

## 参数
* **METHOD**：指定生成 pdf 的方式，缺省采用 latexmk。
  * METHOD=latexmk  表示使用 latexmk 的方式生成 pdf（使用 xelatex）。
  * METHOD=xelatex  表示使用 xelatex 引擎编译生成 pdf；
  * METHOD=pdflatex 表示使用 pdflatex 引擎编译生成 pdf。
