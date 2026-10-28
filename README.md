Quantum Machine Learning for Healthcare: Breast Cancer Classification
1. Project Overview

This project explores quantum machine learning for classifying breast cancer data. I compared a classical Support Vector Machine (SVM) with a quantum-kernel SVM to investigate their performance.

2. Problem

The goal is to classify breast cancer data as malignant or benign using machine learning.

3. Dataset

I used the Breast Cancer Wisconsin dataset from Scikit-learn. It contains 569 samples and 30 features describing cell characteristics.

For the direct comparison, I selected 100 samples and used two features: mean radius and mean texture.

4. Methods

Classical model: An SVM with a radial basis function (RBF) kernel.

Quantum model: PennyLane simulated a two-qubit quantum circuit to calculate a quantum kernel. The kernel measures similarity between data points, and an SVM uses those similarities to make predictions.

Both models in the small comparison used the same data split.

5. Results

Metric	Classical SVM	Quantum-kernel SVM
Accuracy	92%	76%
F1 score	0.9231	0.7857

The classical model performed better in this experiment. The results do not demonstrate a quantum advantage.

6. Limitations

The quantum circuit was simulated on a classical computer rather than run on physical quantum hardware. The direct comparison used a small subset of the dataset and only two features. This project is educational research and is not a clinically validated diagnostic tool.

7. Conclusion

This experiment helped me explore how quantum kernels can be combined with classical machine learning. Future work could test different feature selections, quantum circuit designs, and data splits.

8. Tools Used

* Python
* Google Colab
* Scikit-learn
* PennyLane
* NumPy
* Pandas
* Matplotlib

9. Project Files

* Quantum_healthcare_challenge.ipynb — contains the code, model comparison, chart, and project report.
