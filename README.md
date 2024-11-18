give# Eval-CA-Robustness-PCC-Paper

# Enhancing Corruption Robustness for Point Cloud Classifiers

Point cloud data is widely used to represent 3D objects in applications such as advanced driver assistance systems (ADAS). However, real-world scenarios often introduce corruptions in point cloud data due to factors like rain or sensor noise. These corruptions can mislead AI models that rely on point cloud data, highlighting the need for robust classification systems. This project focuses on improving corruption robustness in point cloud classifiers through adversarial training, a well-established method for enhancing model robustness against adversarial attacks.

## Key Contributions

1. **Adversarial Training with APGD**  
   - Implemented adversarial training using Auto-Projected Gradient Descent (APGD) within the Dynamic Graph Convolutional Neural Network (DGCNN) architecture.  
   - Demonstrated that this approach outperforms other DGCNN models using standard data augmentation techniques in terms of both corruption and adversarial robustness.

2. **Robustness Evaluation**  
   - Evaluated adversarial robustness across various pre-trained point cloud classifiers.

3. **Corruption vs. Adversarial Robustness Analysis**  
   - Explored the relationship between corruption robustness and adversarial robustness to provide deeper insights into their interplay.

## Technical Implementation

The core of this project involved adapting adversarial training for point cloud classifiers using the AutoAttack framework, which introduced APGD as an effective evasion attack method. The implementation included:

- **Modifying APGD for Point Clouds:** Updated AutoAttack’s APGD implementation to handle point cloud data, enabling its use for perturbation generation.  
- **Incorporating APGD into Training:** Integrated the modified APGD into the training phase of point cloud classifiers. Following the adversarial training methodology proposed by Madry et al., APGD-generated perturbations were applied iteratively during training to enhance robustness.  
- **Testing and Analysis:** Conducted extensive experiments to measure robustness improvements, focusing on both adversarial and corruption scenarios.

This project highlights a systematic approach to improving the robustness of point cloud classifiers, paving the way for more reliable AI systems in challenging real-world environments.
