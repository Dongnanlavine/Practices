## Practice 2(15)

**Python and Interactive Computing**：The Simple Simulator of Rankine Cycle 

Deadline: 2019.04.21

## Goal

Use **Jupyter Notebook** to simulate the Rankine Cycle 

* description of the objects with the structure types，abstraction of procedure with functions 

* interactive analysis and literate programming

## 要求：(15)

设计分析 [Example 8.6：The Reheat–Regenerative Cycle with Two Feedwater Heater](./rankine86.md) 的Jupyter Notebook。

合理组织Notebook中的文档(Markdown Cell)和代码(Code Cell)。如：先给出被计算对象描述，然后，给出总体设计思路，进一步是各部分程序模块说明文字、代码，最后，是设计小结。
    
### Jupyter Notebook中的代码(10)

参考 [RankineCycle：SimVer](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-2-PyThermo-RankineCycle-SimVer.ipynb) 和 [RankineCycle：AdvVer](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-3-PyThermo-RankineCycle-AdvVer.ipynb)  

* 使用结构数据类型：**列表、字典**等描述循环中的状态点，设备和循环性能指标(4)

* 基于数据结构的设计，使用**函数**封装计算模块，组织循环计算(3)

* 参考循环计算结果输出： [rankine86-sp.txt](./data/rankine86-sp.txt)，在Jupyter Notebook中输出工整的循环参数和性能指标等结果(3)

* **可选：** 使用数据文件作为循环分析软件的输入输出

   * 参考循环状态点(节点:nodes)数据文件： [rankine86-nd.csv](./data/rankine86-nd.csv) 

   * 参考设备数据文件： [rankine86-de.csv](./data/rankine86-de.csv) 

### Jupyter Notebook中的文档(5)   
    
 **格式(1)**
 
原则上采用Markdown，如果需特殊效果，可少量使用HTML/CSS; 公式用LaTeX(Math)

**内容**： 

问题描述(1)；设计思路(1)； 模块说明(1)；小结(1) 

## 工作提示

1. 阅读、运行和分析 [RankineCycle：SimVer](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-2-PyThermo-RankineCycle-SimVer.ipynb) 和 [RankineCycle：AdvVer](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-3-PyThermo-RankineCycle-AdvVer.ipynb)，熟悉语言和设计思路

2. 阅读和运行 [RankineCycle86-Step0.ipynb](./RankineCycle86-Step0.ipynb) 熟悉分析对象

3. `Make a copy` [RankineCycle86-Step0.ipynb](./RankineCycle86-Step0.ipynb) 为`*-Copy1.ipynb`, 然后，重命名为设计用ipynb文件，如：`03016???-P2.ipynb`

4. 一般设计：可参考[RankineCycle：SimVer](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-2-PyThermo-RankineCycle-SimVer.ipynb)，使用List,Dict和Function做较简单的抽象，编程实现计算，以后再逐步改进。

5. 更好设计：可参考[RankineCycle：AdvVer](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-3-PyThermo-RankineCycle-AdvVer.ipynb)。基于此设计思路的要点是：`新设备`程序设计的如下4个方面：

   * 1 设备的字典描述及计算函数; 2 增加设备到系统设备字典；3 从数据文件生成系统设备字典；4 基于系统设备字典的循环计算

6. 完善ipynb中的文字内容

7. `一般设计` 基本要求，做好可以有满意分数。`更好设计` 给有时间和兴趣，目标是满分的同学。


## Directories and Files

```bash
 ├──<Practices>
 │   │ 
 │   |── <P2>
 │   │    │ 
 │   │    |── start.bat (内容为jupyter notebook的bat文件)
 │   │    │ 
 │   │    |── *.ipynb  (Example 8.6循环分析ipynb文件)
 │   │    |
          |── <data> 存放数据文件
          │        |
          │        │ ── *.csv/txt
          │    
          |── <img> 存放ipynb文件中使用的图片文件
                 |
                 │ ── *.jpg/png
``` 

## 提交：

* 1 电邮： cmh@seu.edu.cn
   
  * 主题：学号-姓名-2
  * 附件：压缩工作目录(如：P2)，命名为： **学号-姓名-2.zip**

* 2 **截至时间：** 2019.04.21
  
  * 截至时间后补交，补交得分<10. (2019.06.16)

* 3 改进更新：提交作业后可改进，改进截至时间：2019.06.16

## Reference：

* Michael J. Moran, Howard N. Shapiro, Daisie D. Boettner, Margaret B. Bailey. Fundamentals of Engineering Thermodynamics(7th Edition). John Wiley & Sons, Inc. 2011
   
   * The ebook at SEU http://www.lib.seu.edu.cn/

     查找资源->外文电子书->Wiley电子教材->T(工业技术)->TK(能源与动力工程)->TK1(热力工程,热机)

* [Markdown](https://github.com/PySEE/home/blob/S2019/guide/Introduction2Markdown(Chinese).md)

* Jupyter 

    * Documentation. http://jupyter.readthedocs.org/en/latest/
    
    * IPython https://ipython.org/
    
    * A gallery of interesting notebook：https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks

* [LaTeX Math](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-3-PyThermo-LaTeX-Math.ipynb)

* [IAPWS-IF97 high-speed shared library:SEUIF97](https://github.com/PySEE/SEUIF97)

* [Unit2-2-PyThermo-RankineCycle](https://nbviewer.jupyter.org/github/PySEE/home/blob/S2019/notebook/Unit2-2-PyThermo-RankineCycle.ipynb)




  

