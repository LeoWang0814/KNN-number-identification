# KNN-number-identification
Using KNN Algorithm to Identify Hand Written Numbers

## 📦 KNN Number Identification | 基于 KNN 的手写数字识别

[![License](https://img.shields.io/github/license/LeoWang0814/KNN-number-identification?style=flat-square)](https://github.com/LeoWang0814/KNN-number-identification/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/LeoWang0814/KNN-number-identification?style=flat-square)](https://github.com/LeoWang0814/KNN-number-identification/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/LeoWang0814/KNN-number-identification?style=flat-square)](https://github.com/LeoWang0814/KNN-number-identification/commits)

> ✨ A simple and educational KNN-based handwritten digit recognition project using Pygame and NumPy.
> ✨ 一个基于 KNN 算法、自制数据集与 Pygame 的手写数字识别小项目，适合作为机器学习入门示例。

---

### 📌 项目简介 | Project Overview

本项目是一个使用 **K 最近邻（K-Nearest Neighbors, KNN）算法** 实现的手写数字识别系统，用户可以通过画板手动绘制数字，程序会通过已有的数字模板进行识别。主要特性如下：

* ✅ 使用 Pygame 实现的简易手写界面
* ✅ 手写输入自动转为 20x20 像素灰度矩阵
* ✅ 基于 KNN 原理对数字进行分类识别
* ✅ 使用 Python 及 NumPy、SciPy 实现图像处理逻辑
* ✅ 便于教学与理解的纯 Python 实现

---

### 🧰 环境依赖 | Environment Requirements

```bash
python >= 3.7
pygame
numpy
scipy
```

使用 pip 快速安装依赖：

```bash
pip install -r requirements.txt
```

> 💡 可手动创建 `requirements.txt` 包含：
>
> ```
> pygame
> numpy
> scipy
> ```

---

### 🚀 如何运行 | How to Run

1. 克隆本项目：

   ```bash
   git clone https://github.com/LeoWang0814/KNN-number-identification.git
   cd KNN-number-identification
   ```

2. 运行主程序：

   ```bash
   python main.py
   ```

3. 手写输入：

   * 鼠标左键按住并绘制数字。
   * 关闭窗口后，程序将自动进行数字识别。

---

### 🧠 识别原理 | Recognition Logic

* **数据预处理**：将绘图转为 20×20 像素矩阵，并进行缩放与裁剪。
* **距离计算**：使用欧几里得距离计算与训练样本的相似度。
* **KNN 分类**：使用固定的训练样本（如数字 0、1）进行最近邻投票。

---


### 📚 文件结构 | Project Structure

```
.
├── main.py                # 主程序入口，包含 UI、预处理、KNN 主逻辑
├── README.md              # 项目说明
├── LICENSE                # 项目许可证
└── requirements.txt       # Python 依赖
```

---

### 🔍 后续改进建议 | Future Improvements

* ✅ 添加更多数字样本（0–9）
* ✅ 实现动态 K 值选择与调优
* ✅ 使用 sklearn 重构为更强健的模型
* ✅ 导入 MNIST 数据集对比效果

---

### 📄 许可证 | License

本项目基于 [MIT License](https://opensource.org/licenses/MIT) 开源，欢迎自由使用、学习与改进。

---

### 🙌 致谢 | Acknowledgments

感谢 [pygame](https://www.pygame.org/) 与 [NumPy](https://numpy.org/) 社区提供强大的工具，使得本项目的开发变得简单易行。
