# 🤖 Multi Model AI Agent with Copilot Studio

Copilot Studio를 활용하여 구축한 Multi Model AI Agent 프로젝트입니다.
사용자의 질문과 요청에 따라 적절한 AI 모델을 활용하여 응답을 생성하며, 
GitHub Pages를 통해 웹 환경에서 접근할 수 있도록 배포하였습니다.

## 📌 프로젝트 개요

본 프로젝트는 Microsoft Copilot Studio를 기반으로 AI Agent를 구현한 사례입니다.
주요 목표는 다음과 같습니다.

- 자연어 기반 사용자 요청 처리
- 다양한 AI 모델 활용(Multi Model)
- 대화형 인터페이스 제공
- GitHub Pages를 통한 간편한 배포

## 🚀 주요 기능
### 1. 사용자의 목적, 난이도, 필요한 응답 속도, 예상 작업 길이를 판단한다.
### 2. 실제 내용 생성과 문제 해결은 가장 적합한 connected agent 한 개에 위임한다.
### 3. 한 에이전트로 충분하면 여러 에이전트를 불필요하게 연속 호출하지 않는다.
### 4. 요청이 불명확해도 안전하게 진행할 수 있으면 합리적인 가정을 한 문장으로 밝히고 진행한다.
### 5. 결과를 크게 바꾸는 정보가 없을 때만 짧게 확인한다.

## 🛠️ 기술 스택

- Microsoft Copilot Studio
- Azure AI Services
- GitHub Pages
- HTML
- JavaScript
- CSS

## 🏗️ 아키텍처

```text
사용자
   │
   ▼
GitHub Pages
   │
   ▼
Copilot Studio Agent : Multi Model AI Agent
   │
   ├── CA1 : Claude Sonnet 5
   ├── CA2 : Claude Opus 5
   ├── CA3 : GPT 5.5 - Chat
   └── CA4 : GPT 5.6 - Reasoning
   │
   ▼
응답 생성
```

## 📂 프로젝트 구조

```text
.
├── index.html
├── css
├── js
└── README.md
```
## 자동 라우팅 규칙

### - 빠른 일반 답변, 요약, 번역, 이메일·안내문 초안, 자연스러운 대화와 짧은 글쓰기는 /CA1-Claude Sonnet5에 위임한다.
### - PPT 제작, 장문 분석, 복합 문서 검토, 섬세한 글쓰기, 높은 문장 완성도와 여러 관점의 종합이 필요한 작업은 /CA2-Claude Opus5에 위임한다.
### - 범용 질의응답, 브레인스토밍, 아이디어 정리, 일상적인 학교생활 도움은 /CA3-GPT-5.5 Chat에 위임한다.
### - 복잡한 추론, 수학·과학 문제 풀이, 코딩, 디버깅, 알고리즘, 다단계 계획과 엄밀한 검증은 /CA4-GPT-5.6 Reasoning에 위임한다.

## 🌐 배포 주소

GitHub Pages URL:

```
https://saturn417.github.io/ai/
```

## 📸 화면 예시

프로젝트 화면 캡처를 추가하세요.

```text
<img width="933" height="860" alt="image" src="https://github.com/user-attachments/assets/594ebe00-a4f7-4092-9b25-8c2a55ac1fbf" />

```

## 📚 참고 자료

- Microsoft Copilot Studio
- Microsoft Learn
- GitHub Pages Documentation

## 👨‍💻 제작자

saturn417

---

본 프로젝트는 Copilot Studio 학습 및 실습 목적으로 제작되었습니다.
