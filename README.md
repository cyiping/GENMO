🚀 NVIDIA 發表 GENMO：人類動作的「通才模型」登場！
你知道嗎？以前 AI 想生成角色動作、或從影片估出 3D 骨架，要用兩個不同模型。
 現在 NVIDIA 把這兩件事「合而為一」——推出 GENMO（Generalist Model for Human Motion） 🎯
這是一個能「看影片就還原 3D 動作」又能「根據文字、音樂或關鍵姿勢生成全新動作」的通用模型。
它同時懂：
🎥 從影片估出全身 3D 動作與攝影機移動
💃 聽音樂生舞蹈、看文字生動作
✋ 依照 3D 關鍵姿勢或 2D 骨架引導
🧩 不同條件可以「時間軸混搭」，自動銜接過場！
 這對機器人學習來說，它可以把人類影片變成可學習的 3D 動作資料。
 這讓「人類動作理解」與「AI 動作創作」終於能在同一模型中協同。
📘 更多資訊：
ICCV 2025 Highlight 論文 https://research.nvidia.com/labs/dair/genmo/......

<p align="center">
 <h1 align="center"> GENMO: A Generalist Model for Human Motion</h1>
  <p align="center">
    <a href="https://jeffli.site/"><strong>Jiefeng Li</strong></a>
    ·
    <a href="https://www.jinkuncao.com/"><strong>Jinkun Cao</strong></a>
    ·
    <a href="https://cs.stanford.edu/~haotianz/"><strong>Haotian Zhang</strong></a>
    ·
    <a href="https://davrempe.github.io/"><strong>Davis Rempe</strong></a>
    ·
    <a href="https://jankautz.com/"><strong>Jan Kautz</strong></a>
    ·
    <a href="https://www.umariqbal.info/"><strong>Umar Iqbal</strong></a>
    ·
    <a href="https://ye-yuan.com/"><strong>Ye Yuan</strong></a>
  </p>
  <h2 align="center">ICCV 2025 (Highlight)</h2>
  <div align="center">
    <img src="./assets/teaser.png" alt="Logo" width="100%">
  </div>
</p>
<p align="center">
  <a href="https://research.nvidia.com/labs/dair/genmo/"><img src="https://img.shields.io/badge/Project-Page-0099cc"></a>
  <a href="https://arxiv.org/abs/2505.01425"><img src="https://img.shields.io/badge/arXiv-2505.01425-b31b1b.svg"></a>

</p>

**GENMO** is a generalist model for human motion that handles multiple tasks with a single model, supporting diverse conditioning signals including video, keypoints, text, audio, and 3D keyframes.

---

## 📰 News

- **[October 2025]** 📢 The **GENMO** codebase is **released!**  
  Stay tuned for the pretrained models and evaluation scripts.  
  Follow the [project page](https://research.nvidia.com/labs/dair/genmo/) for updates and announcements.


---

## 🚀 Highlights

GENMO introduces a **unified generative framework** that connects motion estimation and generation through shared objectives.

- **Unified framework:** Reframes motion estimation as *constrained generation*, allowing a single model to perform both tasks.  
- **Regression × Diffusion synergy:** Combines the accuracy of regression models with the diversity of diffusion-based generation.  
- **Estimation-guided training:** Trains effectively on in-the-wild datasets using only 2D or textual supervision.  
- **Multimodal conditioning:** Supports video, text, audio, 2D/3D keyframes, or even time-varying mixed inputs (e.g., video → text → video).  
- **Arbitrary-length motion:** Generates continuous, coherent sequences of any duration in one diffusion pass.  
- **State-of-the-art performance:** Achieves leading results on diverse motion estimation and generation benchmarks.

For more details, visit the **[GENMO project page →](https://research.nvidia.com/labs/dair/genmo/)**

---

## 📖 Paper & Citation

**Paper:**  
[GENMO: A GENeralist Model for Human MOtion](https://arxiv.org/abs/2505.01425)  
*Jiefeng Li, Jinkun Cao, Haotian Zhang, Davis Rempe, Jan Kautz, Umar Iqbal, Ye Yuan*  
ICCV, 2025

**BibTeX:**
```bibtex
@inproceedings{genmo2025,
  title     = {GENMO: A GENeralist Model for Human MOtion},
  author    = {Li, Jiefeng and Cao, Jinkun and Zhang, Haotian and Rempe, Davis and Kautz, Jan and Iqbal, Umar and Yuan, Ye},
  booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
  year      = {2025}
}
