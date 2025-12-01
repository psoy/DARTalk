![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![LangChain](https://img.shields.io/badge/LangChain-RAG-orange.svg)
![OpenDART](https://img.shields.io/badge/Data-OpenDART-red.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)


# DARTalk
🇰🇷 Korean Corporate Disclosure RAG System: OpenDART API, LangChain, Vector DB를 활용한 한국어 특화 금융 공시 질의응답 솔루션

제목: Dart-RAG-Chatbot (DART 공시 기반 AI 분석 에이전트)
[Project Description]
본 프로젝트는 방대하고 복잡한 **DART(전자공시시스템)**의 기업 공시 문서를 일반 투자자가 쉽고 빠르게 이해할 수 있도록 돕는 RAG(Retrieval-Augmented Generation) 기반 챗봇 시스템입니다.
OpenDART API를 통해 수집된 비정형 데이터(사업보고서, 공시 원문)를 벡터화하여 저장하고, 사용자의 자연어 질문에 대해 근거(Source)에 기반한 정확한 답변을 제공합니다. 금융 도메인에 특화된 전처리 및 검색 로직을 적용하여 할루시네이션을 최소화했습니다.
[Key Features]
🔍 실시간 공시 검색: OpenDART API 연동을 통한 최신 기업 공시 데이터(사업보고서, 현황 등) 자동 수집
🤖 RAG 기반 질의응답: LangChain & Vector DB를 활용해 수백 페이지의 문서 중 핵심 정보를 추출하여 답변 생성
📄 근거 제시 (Source Tracking): 답변의 신뢰도를 높이기 위해 참조한 공시 문서의 원문 링크 및 위치 제공
📊 재무 데이터 해석: 텍스트뿐만 아니라 표(Table) 데이터를 문맥에 맞게 해석하여 재무 상태 요약
[Tech Stack]
Data: OpenDART API, PyDART
LLM & RAG: LangChain, OpenAI GPT-4o / HyperCLOVA X, ChromaDB/Pinecone
Backend: FastAPI, Python
Frontend: Streamlit / React
