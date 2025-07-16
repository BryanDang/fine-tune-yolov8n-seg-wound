# Fine-tune YOLOv8n-seg for Wound Segmentation: A Clinical AI Detective Story

## For Clinician Scientists: Your Gateway to Practical AI Development

This repository contains a comprehensive Jupyter notebook that teaches clinical AI development through a real-world wound segmentation project. More than just code, it's a detective story revealing how even well-regarded datasets can harbor critical flaws that compromise patient care.

## What You'll Learn

### Technical Skills
- **Dataset Auditing**: How to detect hidden biases in medical datasets (discovering a 160:1 class imbalance)
- **Model Training**: Fine-tuning state-of-the-art YOLOv8 for clinical applications
- **AI Interpretability**: Using Grad-CAM to understand what your model actually learns
- **Mobile Deployment**: Quantization techniques to run AI on clinical devices (3.3MB model, 83ms inference)

### Clinical Insights
- Why models can achieve "good" metrics (68% mAP) while learning completely wrong strategies
- How data imbalance leads to edge detection instead of semantic understanding
- The critical importance of clinician involvement in AI development
- Real-world deployment considerations for clinical settings

## Why This Matters

As a nurse scientist who transitioned into AI, I've seen firsthand how clinical expertise is essential for building trustworthy medical AI. This notebook demonstrates:

1. **The Danger of Blind Trust**: A model trained on 2,208 "wound images" learned to detect edges, not wounds
2. **The Power of Clinical Insight**: Only a clinician would recognize zero false positives as suspicious
3. **The Path Forward**: How nurses and clinicians must lead AI development, not just adopt it

## The Story Arc

1. **Train baseline model** → 68.7% mAP (seemingly reasonable)
2. **Clinical suspicion** → Zero false positives? That's not normal
3. **Data investigation** → Discover extreme 160:1 positive/negative imbalance
4. **Form hypothesis** → Model learned edge detection, not wound recognition
5. **Scientific verification** → Grad-CAM reveals focus on boundaries only
6. **Clinical remediation** → Balanced retraining with augmentation
7. **Bedside deployment** → Quantized model ready for mobile use

## Technical Contributions

- **Manual Grad-CAM Implementation**: Bypassing library limitations for YOLOv8 interpretability
- **Systematic Dataset Auditing**: Framework for detecting hidden biases
- **Clinical Deployment Pipeline**: From research to bedside-ready model

## For My Nursing Colleagues

The "nursing shortage" isn't about lack of nurses—it's systemic understaffing. As AI begins automating clinical tasks, we have a choice: shape these tools with our patient-centered expertise, or let others build systems that don't understand bedside care.

This notebook is your invitation to the development table. Because if we don't design the future of nursing, someone else will.

## Getting Started

1. Open the notebook in Google Colab
2. Enable GPU runtime (Runtime → Change runtime type → GPU)
3. Upload your Kaggle API key
4. Run cells sequentially to experience the investigation

## Contact

**Bryan K. Dang, MS, BSN, RN, PHN**  
Nurse Scientist | AI Developer | Patient Advocate

*"The future of clinical AI depends on clinicians who code, not just coders who claim to understand clinical work."*

---

**Note**: This repository supports my graduate capstone project on clinical AI development. The goal is not just to build models, but to empower clinicians to lead AI development with the same dedication they bring to patient care.