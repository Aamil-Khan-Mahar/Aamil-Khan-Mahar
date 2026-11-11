<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=210&color=0:0f0c29,50:302b63,100:24243e&text=Aamil%20Khan%20Mahar&fontColor=ffffff&fontSize=56&fontAlignY=36&desc=statistics%20%E2%88%A9%20engineering&descAlignY=58&descSize=20&animation=fadeIn" width="100%" alt="Aamil Khan Mahar" />

# 𝓐𝓪𝓶𝓲𝓵 𝓚𝓱𝓪𝓷 𝓜𝓪𝓱𝓪𝓻

<a href="https://github.com/Aamil-Khan-Mahar"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=2800&pause=900&color=A78BFA&center=true&vCenter=true&width=620&lines=Data+Scientist+%40+Afiniti;Bayesian+ensembles+in+production;LLM+agents+that+do+real+work;Economics+%2B+Mathematics+%2B+CS;argmin+over+boring+problems" alt="Typing intro" /></a>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/aamil-khan-mahar)
[![Portfolio](https://img.shields.io/badge/Portfolio-302b63?style=for-the-badge&logo=vercel&logoColor=white)](https://aamilkhanmahar-aamil-khan-mahars-projects.vercel.app)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/aamil-khan-mahar)

</div>

## 𝓣𝓱𝓮 𝓜𝓸𝓭𝓮𝓵

```python
from typing import Literal
from pydantic import BaseModel, Field, computed_field


class Degree(BaseModel):
    school: str = "LUMS"
    major: str = "Economics & Mathematics"
    minor: str = "Computer Science"
    year: int = Field(2025, ge=2025)
    honours: list[str] = ["Award of Distinction", "Dean's Honour List x3"]


class Aamil(BaseModel):
    role: str = "Data Scientist @ Afiniti"
    based_in: str = "Karachi, PK"
    degree: Degree = Degree()
    models: list[str] = ["Bayesian (Stan)", "tree ensembles", "transformers", "LLM agents"]
    thinks_in: Literal["priors", "posteriors", "gradients"] = "posteriors"
    building: str = "Masters-App: a town of Claude agents doing grad-school admin"
    open_to: list[str] = ["ML research", "agentic AI", "weird datasets"]

    @computed_field
    @property
    def vibe(self) -> str:
        return "statistics ∩ engineering"


print(Aamil().model_dump_json(indent=2))
```

<details>
<summary><b>▶ Run it</b> (validated, I promise)</summary>

```json
{
  "role": "Data Scientist @ Afiniti",
  "based_in": "Karachi, PK",
  "degree": {
    "school": "LUMS",
    "major": "Economics & Mathematics",
    "minor": "Computer Science",
    "year": 2025,
    "honours": ["Award of Distinction", "Dean's Honour List x3"]
  },
  "models": ["Bayesian (Stan)", "tree ensembles", "transformers", "LLM agents"],
  "thinks_in": "posteriors",
  "building": "Masters-App: a town of Claude agents doing grad-school admin",
  "open_to": ["ML research", "agentic AI", "weird datasets"],
  "vibe": "statistics ∩ engineering"
}
```

</details>

## 𝓣𝓱𝓮 𝓞𝓫𝓳𝓮𝓬𝓽𝓲𝓿𝓮

$$
\text{Aamil} \;=\; \underbrace{\text{Economics}}_{\text{why it matters}} \;\otimes\; \underbrace{\text{Mathematics}}_{\text{how it works}} \;\oplus\; \underbrace{\text{CS}}_{\text{ship it}}
$$

$$
\theta^{\ast} \;=\; \arg\min_{\theta}\; \mathbb{E}_{(x,\,y)\,\sim\,\mathcal{D}_{\text{real world}}}\Big[\, \mathcal{L}\big(f_{\theta}(x),\, y\big) \Big] \;+\; \lambda \,\big\lVert \text{overengineering} \big\rVert_2^2
$$

## 𝓣𝓱𝓲𝓷𝓰𝓼 𝓘'𝓿𝓮 𝓑𝓾𝓲𝓵𝓽

| | Project | 𝕋𝕃;𝔻ℝ |
|:-:|---|---|
| 🏘️ | **[Masters-App](https://github.com/Aamil-Khan-Mahar/Masters-App)** | A village of Claude agents (scouts, researchers, a coach) that runs a whole grad-school application cycle. FastAPI, React, TypeScript. |
| 🤖 | **Agentic underperformance analyst** | LangGraph, tool-calling agents on AWS Bedrock with Pydantic outputs that diagnose why production models slip. |
| 🛰️ | **House boundary segmentation** | TransUNet (ResNet50 + ViT-B/16) on aerial imagery, with five loss functions and a diffusion-based edge-refinement step. |
| 🐛 | **DeBuggy** | A four-stage GPT-4o find, fix and test pipeline fed straight from Slack and email: 15 of 15 bugs fixed, about 90% less developer time. |
| 📚 | **RAG research chatbot** | Drop in papers and ask questions: Pinecone retrieval, Mixtral-8x7B, and Wikipedia when the papers don't know. |
| 📰 | **[Urdu news classifier](https://github.com/Aamil-Khan-Mahar/UNA_Categorisation)** | Naive Bayes, logistic regression and a neural net written from scratch, reaching 95.24% accuracy on four outlets. |
| 📈 | **467 LSTMs walk into the NYSE** | One stacked LSTM per ticker, with the forecasts fed into Max-Sharpe portfolios. |
| 🧠 | **From scratch, because why not** | A ViT in PyTorch, a CNN in pure NumPy, CycleGAN (horse to zebra), and knowledge distillation into students under 2M parameters. |
| 🚗 | **License plate reader** | YOLOv8 and EasyOCR with a searchable Streamlit app. |

## 𝓡𝓮𝓼𝓮𝓪𝓻𝓬𝓱

- 🏛️ **LUMS Economics:** research assistant on a [working paper](https://ideas.repec.org/p/new/wpaper/2411.html) reframing Pakistan's monetary system, and builder of a corpus of 5,000+ National Assembly debates from 1947 to 2022.
- 🧪 **LUMS Center for Speech and Language Technologies:** MigraineAid, which predicts migraines from content-blind behavioral signals.

## 𝓣𝓸𝓸𝓵𝓫𝓸𝔁

<div align="center">

<img src="https://skillicons.dev/icons?i=py,pytorch,tensorflow,sklearn,r,postgres,aws,docker&theme=dark" alt="Python, PyTorch, TensorFlow, scikit-learn, R, PostgreSQL, AWS, Docker" />
<br />
<img src="https://skillicons.dev/icons?i=opencv,ts,react,fastapi,nodejs,mongodb,linux,latex&theme=dark" alt="OpenCV, TypeScript, React, FastAPI, Node.js, MongoDB, Linux, LaTeX" />

</div>

## 𝓕𝓾𝓷 𝓕𝓪𝓬𝓽𝓼

<details>
<summary><b>∑ expand</b></summary>

- My degree is a joint major in 𝔼𝕔𝕠𝕟𝕠𝕞𝕚𝕔𝕤 and 𝕄𝕒𝕥𝕙𝕖𝕞𝕒𝕥𝕚𝕔𝕤, so I'm contractually obliged to put an expectation on everything.
- I've read (well, parsed) 75 years of parliamentary debates.
- My resume is built by a pipeline that picks entries by ID and never edits a word.
- One segmentation project, five loss functions (Dice, BCE, Hausdorff, Focal, Lovász). My favourite is whichever one goes down.

</details>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Aamil-Khan-Mahar/Aamil-Khan-Mahar/output/github-snake-dark.svg" />
  <img src="https://raw.githubusercontent.com/Aamil-Khan-Mahar/Aamil-Khan-Mahar/output/github-snake.svg" alt="A snake eating my contribution graph" />
</picture>

<img src="https://capsule-render.vercel.app/api?type=waving&height=110&color=0:24243e,50:302b63,100:0f0c29&section=footer" width="100%" alt="" />

</div>
