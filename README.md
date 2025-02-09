![MatrixHub_logo](./docs/img/MatrixHub_logo.png)

Matrix_hub
=======================================
矩阵运算库--C语言
---------------------------------------
A lib for Matrix Operations in C language. (矩阵运算库--C语言) 

Author: Amoiensis (Xiping.Yu)

Email: Amoiensis@outlook.com

Data: 2020.02.12~2022.05.28

***************************************************************
更多资料和信息：

https://github.com/Amoiensis/Matrix_hub

[[Releases 快速下载]: Matrix_Hub_v1.51.zip](https://github.com/Amoiensis/Matrix_hub/releases/download/v1.51/Matrix_Hub_v1.51.zip)

***************************************************************

具体应用例子：

Optimization-Algorithm(最优化算法)：https://github.com/Amoiensis/Optimization-Algorithm
***************************************************************

具体：
	Folder_--_lib_.lib文件_+_.h文件
	
	Folder_--_code_.c文件_+_.h文件

***************************************************************

[CONTENT](https://github.com/Amoiensis/Matrix_hub)
---------------------------------------

####（操作-函数）
|                     操作                      |    Func Name     |                     Operation (detailed)                     |
| :-------------------------------------------: | :--------------: | :----------------------------------------------------------: |
|                   生成矩阵                    |    Matrix_gen    |                   Generate  a new Matrix.                    |
|                   复制矩阵                    |   Matrix_copy    |                    Copy  to a new Matrix.                    |
|                     乘法                      |      M_mul       |    Matrix  multiplication (create new one, abbr. create).    |
|                    加减法                     |    M_add_sub     |               Addition/  subtraction (create).               |
|                   矩阵显示                    |     M_print      |                       Print,  Display.                       |
|                单位矩阵(生成)                 |       M_I        |            Generate  a identity Matrix (create).             |
|                 矩阵基本变换                  |    M_E_trans     |              Matrix  elementary transformation.              |
|                 基本变换矩阵                  | Etrans_2_Matrix  | Transforms  the elementary transformation into Matrix (create). |
|             基本变换矩阵的逆矩阵              | Etrans_4_Inverse |   Inverse  Matrix of elementary transformations (create).    |
|                   上三角化                    |     M_Uptri_     | Upper-Triangulation  transformation on the Matrix (create).  |
|               上三角化(求逆用)                |   M_Uptri_4inv   | For  inverse, upper-triangulation transformation on the Matrix (create). |
|                   下三角化                    |    M_Lowtri_     | Lower-Triangulation  transformation on the Matrix (create).  |
|               下三角化(求逆用)                |  M_Lowtri_4inv   | For  inverse , lower-triangulation transformation on the Matrix (create). |
|                 对角矩阵求逆                  |    M_Dia_Inv     |        The  inverse of the diagonal Matrix (create).         |
|                    对角化                     |    M_Diatri_     |                  Diagonalization  (create).                  |
|                     求逆                      |    M_Inverse     |                      Inverse  (create).                      |
|                矩阵行(列)调换                 |      M_Swap      |              Swap  row or cloumn of the Matrix.              |
|                     转置                      |       M_T        |                     Transpose  (create).                     |
|                 切取部分矩阵                  |      M_Cut       |       Cut out a part-matrix from the Matrix (create).        |
|                   释放内存                    |      M_free      |           Free  the memory of the Matrix (create).           |
|                      迹                       |       M_tr       |                            Trace.                            |
|                    行列式                     |      M_det       |                         Determinant.                         |
|                     填充                      |      M_full      |             Full  the Matrix with data (create).             |
|                     范数                      |      M_norm      |                  Norm  (1/ 2/ p/ INF/ FRO).                  |
|                  矩阵绝对值                   |      M_abs       |   Absolute  the value of elements in the Matrix  (create).   |
|                   矩阵数乘                    |     M_numul      |               Number  Multiplication (create).               |
|              (使用矩阵)填充矩阵               |    M_matFull     |            Full  the Matrix with another Matrix.             |
|                生成(全)零矩阵                 |     M_Zeros      |            Generation  All-Zeros-Matrix (create).            |
|                生成(全)一矩阵                 |      M_Ones      |            Generation  All-Ones-Matrix (create).             |
|          寻找矩阵对应值位置(列优先)           |      M_find      | Find  all the positions with a certain value in the Matrix (create). |
|            矩阵按列求和/向量元素和            |      M_sum       | Matrix  Column-Summation (create). / Vector element Sum (create) . |
|   矩阵按列最小行位置     /向量最小元素位置    |      M_min       | Minimum-value position for each row in  the Matrix (create) .  / Vector minimum element position (create) . |
|   矩阵按列最大行位置     /向量最大元素位置    |      M_max       | Maximum-value position for each row in  the Matrix (create)./ Vector Maximum element position (create) . |
|            矩阵各列指定行位置的值             |   M_minax_val    | The value of those given (row) positions for each column in the matrix (create). |
| 矩阵各位置与给定值比较     (返回矩阵,取值0/1) |  M_logic_equal   | Compare every element /pisition of the  Matrix with certain value (create).     [ More : Return a new Matrix, whose every value is 0/1. ] |
|            两矩阵对应位置逻辑运算             |     M_logic      | Logical  operation of corresponding positions of two matrices |
|         矩阵对应元素乘/除 (哈达玛积)          |    M_pmuldiv     | Hadamard  Product : Multiply / Divide every element in the two Matrix-s (create). |
|          矩阵批量赋值(使用矩阵传递)           |     M_setval     |       Setting  Values of a Matrix with another Matrix.       |
|          矩阵对矩阵，对各行进行数乘           |    M_numul_m     |    Matrix  Number Multiplication (using matrix transfer)     |
|                   矩阵求秩                    |      M_rank      |                            Rank.                             |
|      (函数: M_rank) 释放初等变换内存空间      |   Etrans_free    | (In  Func: M_rank) Free memory for Elementary Transformation. |
|                 矩阵求条件数                  |      M_cond      |                Conditon  Value of the Matrix.                |
|               生成希尔伯特矩阵                |     Hilbert      |              Generate  Hilbert Matrix (create).              |
|           矩阵最大特征值、特征向量            |   M_eigen_max    | The maximum eigenvalue/ eigen-vector of the Matrix (create). |
|      向量householder变换, 返回变换矩阵H       |   householder    | Householder transformation for  the Vector, return Transformating-Matrix: H (create). |
|              矩阵householder变换              |  M_householder   | Householder transformation for  the Matrix, return Transformated-Matrix: H_Mat (create). |
|                  矩阵QR分解                   |       M_QR       |                  QR Decomposition (create).                  |
|                  矩阵特征值                   |   M_eigen_val    |           The eigenvalues of the Matrix (create).            |
|      矩阵特征值, 及其对应特征向量(矩阵)       |     M_eigen      |  The eigenvalues and eigen-vectors of the Matrix (create).   |
|                     帮助                      |       help       |                            Help.                             |


Demo.c (Matrix_hub)
---------------------------------------

```
/*
\ \     __  ___     __      _       __ __     __
 \ \   /  |/  /__ _/ /_____(_)_ __ / // /_ __/ /
 / /  / /|_/ / _ `/ __/ __/ /\ \ // _  / // / _ \
/ /  /_/  /_/\_,_/\__/_/ /_//_\_\/_//_/\_,_/_.__/
* [INFORMATION]
    MATRIX_HUB
    AUTHOR: Xiping.Yu
    E-MAIL:Amoiensis@outlook.com
    GITHUB: https://github.com/Amoiensis/Matrix_hub
    DATE: 2020.02.12-2022.05.28
    VERSION: 1.5.1
    CASE: Matrix Operation (C)
    DETAILS: The demo-code for Matrix_Hub.
    LICENSE: Apache-2.0
*/

#include <stdio.h>
#include <stdlib.h>
#include "matrix.h"


int main(int argc, char *argv[]) {

//  Matrix
    //	Mat_1
    ...
    [ 具体矩阵赋值，见 demo.c ]

//	Operation
    // 乘法
    Matrix *mat_3 = M_mul(mat_2, mat_1);
    M_print(mat_3);
    // 加减法
    Matrix *mat_diff = M_add_sub(1, mat_21, 1, mat_21b);
    M_print(mat_diff);
    // 单位矩阵
    M_print(M_I(5));
    // 上三角变换
    Uptri_struct *_Uptri_ = M_Uptri_(mat_21);
    M_print(_Uptri_->trans_matrix);
    M_print(_Uptri_->Uptri_matrix);
    // 下三角变换
    Lowtri_struct *_Lowtri_ = M_Lowtri_(mat_21);
    M_print(_Lowtri_->Lowtri_matrix);
    M_print(_Lowtri_->trans_matrix);
    // 对角化
    Dia_struct *_Dia_ = M_Diatri_(mat_21);
    M_print(_Dia_->trans_leftmatrix);
    M_print(_Dia_->Diatri_matrix);
    M_print(_Dia_->trans_rightmatrix);
    // 矩阵求逆
    Matrix *_mat_inv = M_Inverse(mat_21);
    M_print(_mat_inv);
    // 行列交换
    M_Swap(_mat_inv, 1, 2, _ROW_);
    M_print(_mat_inv);
    // 切割部分
    Matrix *_mat_cut = M_Cut(_mat_inv, _END_, _END_, 2, 3);
    M_print(_mat_cut);
    // 转置
    Matrix *_mat_T = M_T(_mat_inv);
    M_print(_mat_T);
    // 迹
    MATRIX_TYPE _tr_mat = M_tr(_mat_inv);
    printf("Tr(Matrix_%x) = %.4lf\n", _mat_inv, _tr_mat);
    // 行列式
    MATRIX_TYPE _det_mat = M_det(_mat_inv);
    printf("Det(Matrix_%x) = %.4lf\n", mat_21, _det_mat);
    // 填充
    Matrix *mat_full = M_full(mat_2, 1, 1, 1, 1, 0);
    M_print(mat_full);
    // 范数
    printf("NORM1 = %lf\n", M_norm(mat_b, 1));
    printf("NORM2 = %lf\n", M_norm(mat_b, 2));
    // 秩
    printf("Rank(%x) = %d\n", mat_A10, M_rank(mat_A10));
    printf("Rank(%x) = %d\n", mat_full, M_rank(mat_full));
    // Hilbert 希尔伯特矩阵
    printf(">> Gen Hilbert-Matrix\n");
    M_print(Hilbert(5));
    // 求条件数
    printf("条件数为: %lf\n", M_cond(Hilbert(5),1));
    //  矩阵QR分解
    Matrix * M_H = M_householder(Hilbert(5));
    M_print(M_H);
    //  矩阵特征值
    Matrix * M_eigen_I = M_eigen_val(M_H);
    M_print(M_eigen_I);
    // 特征值+特征向量
    Matrix *target = M_H;
    M_print(target);
    Matrix ** M_eigen_val_vec = M_eigen(target);
    M_print(M_eigen_val_vec[0]);
    M_print(M_eigen_val_vec[1]);
    // 验证特征值, 特征向量
    M_print(M_mul(target,M_eigen_val_vec[1]));

// Application
    // 解线性方程
    // mat_A*x = mat_b
    printf("#Solver:mat_A*x = mat_b\n");
    Matrix *_mat_result = M_mul(M_Inverse(mat_A10), mat_b10);
    M_print(_mat_result);
    // 测试 Hilbert 希尔伯特矩阵(病态矩阵)
    // Hilbert(n)*x = One(n,1)
    int order = 10;
    printf("#Solver:Hilbert(%d)*x = One(%d,1)\n", order, order);
    M_print(M_mul(M_Inverse(Hilbert(order)), M_Ones(order,1)));
    // 测试希尔伯特矩阵的秩
    printf("Rank(Hilbert(n)) = %d\n", M_rank(Hilbert(5)));

//  Others
    M_free(_mat_T); // 释放矩阵内存
    // [补充] 已修正: 一维矩阵无法实现求逆
    M_print(M_Inverse(M_Zeros(1,1))); // 已验证通过

// Help 函数
    help("help");
    help("M_rank");
    help("Update");
    help("MatrixHub");

    system("pause");
    return 0;
}

```



## [[更新说明]](https://github.com/Amoiensis/Matrix_hub) 

#### [Matrix Hub v1.51] 2022.05.28

1. 新增函数, 详情见下表 M_eigen_max/ householder/ M_householder/ M_QR/ M_eigen_val;

|                操作                |   Func Name   |                     Operation (detailed)                     |
| :--------------------------------: | :-----------: | :----------------------------------------------------------: |
|      矩阵最大特征值、特征向量      |  M_eigen_max  | The maximum eigenvalue/ eigen-vector of the Matrix (create). |
| 向量householder变换, 返回变换矩阵H |  householder  | Householder transformation for  the Vector, return Transformating-Matrix: H (create). |
|        矩阵householder变换         | M_householder | Householder transformation for  the Matrix, return Transformated-Matrix: H_Mat (create). |
|             矩阵QR分解             |     M_QR      |                  QR Decomposition (create).                  |
|             矩阵特征值             |  M_eigen_val  |           The eigenvalues of the Matrix (create).            |
| 矩阵特征值, 及其对应特征向量(矩阵) |    M_eigen    |  The eigenvalues and eigen-vectors of the Matrix (create).   |


2. 新增 运算过程的"显示详细等级"(The Level of Details of Output).

   位置: _DETAILED_ (state.h)
   
   档位: 0/1/2/3 四等级: 0->3 逐渐详细 ( 默认设置为 2级)

   **level - 显示详情的函数**  

   0 - M_print （除设定的输出外，不额外显示其他计算细节信息）  

   1 - M_Uptri_/ M_Lowtri_/ M_Diatri_ ;  

   2 - M_full/ M_Inverse/ M_eigen_val/ M_rank / M_Uptri_/ M_Lowtri_/ M_Diatri_/ M_print ;  

   3 - M_free/ M_mul/ M_full/ M_Inverse/ M_rank/ M_mul / M_Uptri_/ M_Lowtri_/ M_Diatri_/ M_print ;  

3. 解决求逆运算中存在的问题(感谢[@1u2e](https://github.com/1u2e)): 结构体释放问题、一维矩阵求逆;
   详见：https://github.com/Amoiensis/Matrix_hub/issues/4

4. 本版本已完成内存测试，目前测试后暂无内存泄漏问题；

5. 更新"README", 参考"功能表"中 OPERATION 列, 如返回值为新开辟空间则标记有 "create", 用于提供内存管理的参考,
       具体请参考对应 OPERATION 说明 help("README").

6. 自Matrix_Hub v1.51 起, 可以使用 help("MatrixHub") 查看当前版本号.



#### [Matrix Hub v1.50] 2022.04.29

1. 新增函数, 矩阵求条件数 M_cond (matrix.h);

2. 进一步克服 v1.44 内存问题, 完善内存管理, 可使用 help("Memory_Manager") 查看;

   **注意**：本次更新内存管理大幅改善，已修复v1.4x内存问题。



#### [Matrix Hub v1.44] 2022.04.28

1. 新增函数 矩阵求秩: M_rank (matrix.h);

2. 新增函数 Etrans_free, 实现 M_rank 初等变换内存释放; 详见 help("Etrans_free"), (matrix.h)

3. 新增希尔伯特矩阵(病态矩阵)生成: Hilbert (matrix.h);

4. 新增矩阵不可逆报错, Error: M_Dia_Inv_023: "@ERROR: Matrix is not invertible!" (state.h);

5. 已修复 v1.43 计算不稳定问题;

   **注意**：本次更新内存和计算速度都得到提高，已修复v1.43稳定性问题。



#### [Matrix Hub v1.43] 2021.10.26

1. 更新矩阵求逆算法，所有基于求逆的运算速度提升，更新"M_Inverse"函数；

2. 修复初等变换的内存问题，程序运行内存占用减少；

3. 删除“Etrans_2_Inverse”函数；新增“Etrans_4_Inverse”函数，用于加速矩阵求逆；

4. 更新“M_Uptri_4inv”、“M_Lowtri_4inv”用于加速矩阵求逆；

   ~~**注意**：推荐目前请使用 [Matrix Hub v1.42]v1.42版本，本次更新内存和计算速度都得到提高，但是存在一些稳定性问题，正在修复。~~

#### [Matrix Hub v1.42] 2021.08.06

1. 新增求解矩阵最大特征值函数:M_eigen_max()，可使用help("M_eigen_max")查看具体使用；
2. 新增矩阵取绝对值函数 M_abs()，可使用help("M_abs")查看具体使用；
3. 完善向量和矩阵的各种范数运算M_norm()：新增1范数(1)、2范数(2)、无穷范数(INF)、F范数（FRO）等方法，修正了矩阵二范数计算错误的问题,可使用help("M_norm")查看具体使用；

#### [Matrix Hub v1.4] 2021.02.02

1.	新增 help() 函数，可以输入各函数名称，查看具体使用方法；如，help("help")、help("Matrix_gen")、help("README")、help("Update")，等;


2. 	新增函数“M_numul_m ()”，用于矩阵数乘 ，矩阵对于矩阵进行操作，各行对应数乘 ；


3.	将原 M_matFull() 函数中，最左侧，和最上侧，row_up和column_left取值从“0”设置为“1（_HEAD_）”;


4.	修正原代码中"Matirx"的误写，修正为"Matrix";





ATTENTION
---------------------------------------

Please feel free to contact with me for any questions, thank you!

Don't spread the files without permission!

所有文件仅仅供学习交流！

未经允许，请勿传播！

***************************************
