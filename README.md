# SelfCheckGPT Reproduction

SelfCheckGPT 논문의 black-box 환각 탐지 방법 일부를 재현하는 프로젝트입니다. (진행 중)


## 개요
- 논문: Manakul et al.,
- *SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models*,
- EMNLP 2023 (arXiv:2303.08896)
- 데이터: `potsawee/wiki_bio_gpt3_hallucination` (문서 238개, 문장 1,908개, 문서당 샘플 20개)
- 환경: Google Colab (T4 GPU), LLM API 미사용
- 평가: 문장 단위 AUC-PR (accurate = 0, minor/major inaccurate = 1)


## AI 도구 사용 범위
- Unigram 점수 함수, 라벨 이진화, AUC-PR 계산: 직접 작성
- NLI 실행 및 실험 코드: Claude의 도움을 받아 작성
