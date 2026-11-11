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

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=110&color=0:24243e,50:302b63,100:0f0c29&section=footer" width="100%" alt="" />

</div>
