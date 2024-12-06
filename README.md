# Randomly-Sparse-Kernel CNN (RSKCNN)

## Description  
This repository contains the data and model implementation for the research paper titled **"RSKCNN—Introducing Randomly-Sparse-Kernel CNN"** The proposed method introduces a novel sparsity-based optimization technique that improves CNN training speed, accuracy, and generalization performance by reducing data density during convolution operations.

### Key Highlights  
- **Randomly Sparse Kernels**: Implements a Dropout-like operation within convolutional kernels to achieve sparsity.  
- **Improved Performance**: Demonstrates better training speed and reduced overfitting compared to traditional CNNs.  
- **Ease of Use**: The algorithm is simple to integrate and provides additional hyperparameter options for model tuning.  
- **Metrics**: Evaluated on several datasets, showing improvements in FLOPs and validation accuracy.  

---

## Project Structure  
The repository includes the following:  

1. **Models**  
   - Implementation of the RSKCNN algorithm.  
   - Code for integrating sparse convolutional kernels into existing CNN architectures.

2. **Data**  
   - Preprocessed datasets and results from testing RSKCNN on various architectures and hardware platforms.  
   - Comparison metrics with other sparsity techniques, such as SpatialDropout and structured pruning.  

3. **Presentation**  
   - A PowerPoint presentation introducing the RSKCNN method, its key concepts, and experimental outcomes.  

4. **Paper**  
   - The full research paper detailing the methodology, experiments, and findings of the RSKCNN algorithm.

---

## Features  
1. Converts convolutional kernels into sparse kernels using a mask matrix.  
2. Enhances model accuracy by reducing overfitting through a regularization effect.  
3. Reduces computational complexity during convolutions, improving training efficiency.  
4. Offers flexibility for further hyperparameter tuning and customization.  

---

## Limitations  
- Sparse matrix positions with zeros are not fully optimized, leaving potential for further enhancements.  
- Slower convergence requiring additional training iterations.  
- Limited testing on large-scale datasets and architectures.  
- The probability parameter \(p\) for sparsity is manually set and not self-learned.

---

## How to Use  
1. Clone the repository:  
    
```bash
git clone https://github.com/yourusername/RSKCNN.git
cd RSKCNN
```
   
---

## Citation

If you use this repository in your research, please cite our paper:

```bibtex
@inproceedings{rskcnn2024,
  title={RSKCNN—Introducing Randomly-Sparse-Kernel},
  author={Zhexi Feng and Yutao He and Yucheng Li},
  booktitle={Proceedings of the 2024 5th International Conference on Computer Vision and Information Technology (CVIT 2024)},
  year={2024},
  address={Beijing, China},
  month={August 16--18}
}
```

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

Contact

For questions, please contact <f18795465975zx@gmail.com>.


