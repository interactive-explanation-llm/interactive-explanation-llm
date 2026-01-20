# Improving Human Verification of LLM Reasoning through Interactive Explanation Interfaces

[![arXiv](https://img.shields.io/badge/arXiv-2510.22922-b31b1b.svg)](https://arxiv.org/abs/2510.22922)
[![Website](https://img.shields.io/badge/Website-Live-blue)](https://nikitakharya09.github.io/improving-human-verification-of-llm-reasoning/)

Official website for the paper "Improving Human Verification of LLM Reasoning through Interactive Explanation Interfaces" by Runtao Zhou, Giang Nguyen, Nikita Kharya, Anh Totti Nguyen, and Chirag Agarwal.

## 🎯 Overview

Traditional LLMs output static text that is difficult to verify. We introduce three interactive frameworks that transform LLM reasoning into navigable interfaces, making verification **faster** (57.9s vs 64.7s), **more accurate** (85.6% vs 73.5%), and **more reliable** for error detection (85.2% vs 66.1%).

### Three Interactive Frameworks:

1. **iCoT (Interactive Chain-of-Thought)** - Discrete, step-by-step blocks with navigation controls
2. **iPoT (Interactive Program-of-Thought)** - Code-based explanations with variable tracking
3. **iGraph** - Visual node-link diagrams showing computational dependencies ⭐ **Best performer**

## 📊 Key Results

Our user study with **125 participants** demonstrates:

- **+12.1% verification accuracy** (85.6% vs 73.5% baseline)
- **-6.8s faster verification** (57.9s vs 64.7s baseline)
- **+19.1% better error localization** (85.2% vs 66.1% baseline)
- **91% user satisfaction** rating for iGraph

## 🌐 Website

Visit the live website: [https://nikitakharya09.github.io/improving-human-verification-of-llm-reasoning/](https://nikitakharya09.github.io/improving-human-verification-of-llm-reasoning/)

## 📁 Repository Structure

```
├── index.html          # Main website file (self-contained)
├── README.md           # This file
└── LICENSE             # MIT License
```

## 🚀 Local Development

The website is a single self-contained HTML file with no dependencies. Simply:

1. Clone this repository:
   ```bash
   git clone https://github.com/nikitakharya09/improving-human-verification-of-llm-reasoning.git
   cd interactive-llm-verification
   ```

2. Open `index.html` in your browser:
   ```bash
   open index.html  # macOS
   # or
   xdg-open index.html  # Linux
   # or just double-click the file
   ```

## 🌍 Deploy to GitHub Pages

1. Go to your repository on GitHub
2. Navigate to **Settings** → **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**
6. Your site will be live at `https://nikitakharya09.github.io/improving-human-verification-of-llm-reasoning/`

## 📄 Citation

If you find our work useful, please cite:

```bibtex
@article{zhou2025improving,
  title={Improving Human Verification of LLM Reasoning through Interactive Explanation Interfaces},
  author={Zhou, Runtao and Nguyen, Giang and Kharya, Nikita and Nguyen, Anh Totti and Agarwal, Chirag},
  journal={arXiv preprint arXiv:2510.22922},
  year={2025}
}
```

## 👥 Authors

- **Runtao Zhou** - University of Virginia - [uar6nw@virginia.edu](mailto:uar6nw@virginia.edu)
- **Giang Nguyen** - Auburn University - [nguyengiangbkhn@gmail.com](mailto:nguyengiangbkhn@gmail.com)
- **Nikita Kharya** - Independent Researcher - [nikitakharya09@gmail.com](mailto:nikitakharya09@gmail.com)
- **Anh Totti Nguyen** - Auburn University - [anh.ng8@gmail.com](mailto:anh.ng8@gmail.com)
- **Chirag Agarwal** - University of Virginia - [chiragagarwal@virginia.edu](mailto:chiragagarwal@virginia.edu)

## 📝 Paper

- **arXiv**: [https://arxiv.org/abs/2510.22922](https://arxiv.org/abs/2510.22922)
- **PDF**: [Download](https://arxiv.org/pdf/2510.22922.pdf)

## 🔗 Links

- [Interactive Demo](https://huggingface.co/spaces/your-space) *(Coming Soon)*
- [Paper (arXiv)](https://arxiv.org/abs/2510.22922)
- [University of Virginia](https://www.virginia.edu/)
- [Auburn University](https://www.auburn.edu/)

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

We thank all 125 participants in our user study for their valuable feedback and contributions to this research.

---

**Questions?** Feel free to open an issue or contact the authors directly.
