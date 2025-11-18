# Steganalysis ML Project – Phát hiện ẩn mã bằng Học sâu & Học máy

Dự án hoàn chỉnh, chuyên nghiệp, production-ready để phát hiện steganography trong ảnh (LSB, J-UNIWARD, HILL, etc.)

## Tính năng
- Hydra + MLflow quản lý thí nghiệm
- CNN (ResNet, EfficientNet), XGBoost + SPAM features
- Ensemble mạnh nhất
- Demo Streamlit / Gradio / FastAPI
- Docker + CI/CD GitHub Actions
- Reproducible 100%

## Quick Start
```bash
conda env create -f environment.yml
conda activate steg-ml
python scripts/download_data.py --dataset bossbase --payload 0.4
python scripts/train_cnn.py experiment=cnn_augmented model=efficientnet
streamlit run deployment/streamlit_app.py
