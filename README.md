# GPT-SoVITS 語音克隆實作紀錄

## 📌 專案背景 (Project Overview)
本專案為 AI 語音合成的實作練習，旨在掌握從語音數據清洗、音頻切片到模型微調（Fine-tuning）的完整 Pipeline。

## ⚙️ 開發環境 (Environment)
針對本地硬體進行了環境優化與效能測試：
- **GPU**: NVIDIA GeForce RTX 4060 Ti (8GB VRAM)
- **Storage**: C 槽 SSD (優化 I/O 讀取效率，避免訓練時的 Bottleneck)
- **Framework**: PyTorch / CUDA 12.x

## 🛠️ 我的實作內容 (My Contribution)
- **數據集準備**：採集並處理了約 [填入時間，例如：30 分鐘] 的原始語音資料。
- **資料清洗**：使用 UVR5 進行人聲分離，並透過內建腳本完成去噪與 10s 以內的音頻自動切片。
- **模型訓練**：在本地端完成訓練，並針對 [某個音色] 進行了參數調優。

## 📊 遇到的問題與解決方案 (Technical Challenges)
- **問題 A**：(例如：初始環境路徑報錯或 Cuda 版本衝突)
- **解決方案**：(例如：透過 Conda 重新建置獨立環境，並手動指定 Path 位址)

## 🎧 實作成果
(這裡可以放一張 WebUI 執行時的截圖，或是描述訓練出的音質效果)
