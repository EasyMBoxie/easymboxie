# 변경 이력

EasyMBoxie 공개 배포판의 주요 변경 사항을 기록합니다.

이 문서는 GitHub Releases에 첨부되는 실행 파일 기준으로 관리합니다.

## [0.0.7] - 2026-06-11

### 추가

- 공개 배포 및 피드백 수집용 저장소 구성
- 이미지/PDF 등록, OCR 실행, 검수, Publish, WordPress 게시로 이어지는 기본 앱 설명 정리
- GitHub Releases 기반 실행 파일 배포 안내
- 바이너리 평가판 사용 허가서 추가

### 현재 포함된 주요 기능

- Windows x64 데스크톱 앱
- 로컬 우선 OCR/PDF/image 처리 흐름
- PaddleOCR 및 PaddleOCR-VL 기반 OCR/문서 구조 인식
- OCR 실행, 검수, 학습 데이터 관리
- Google Vision 기반 OCR 보정 보조
- OpenAI / Gemini 기반 AI 초안 생성
- AI 결과 편집 및 TXT, Markdown, HTML, JSON, DOCX 내보내기
- WordPress 연결 테스트 및 게시 흐름
- 양식 문서 템플릿 기반 값 추출, 검수, CSV/XLSX 내보내기
- AI 사용량과 외부 API 호출량 확인

### 알려진 사항

- 최초 실행 시 기본 CPU OCR 런타임 준비 화면이 표시될 수 있습니다.
- GPU OCR 환경은 최초 실행 게이트가 아니라 `Settings > OCR 설정 > OCR 환경 설정`에서 별도로 설치/진단합니다.
- 코드 서명 인증서가 적용되어 있지 않아 Windows SmartScreen 또는 백신 프로그램이 새 실행 파일에 대해 경고를 표시할 수 있습니다.
- AI 초안 생성, Google Vision 보정, WordPress 게시 기능은 사용자가 직접 API 키 또는 연결 정보를 설정해야 합니다.
- 초기 공개 배포 단계이므로 기능 이름, 화면 구조, 저장 형식, 배포 방식이 변경될 수 있습니다.

## 기록 방식

각 버전은 가능한 한 아래 분류를 사용합니다.

- `추가`: 새 기능
- `변경`: 기존 기능 변경
- `수정`: 오류 수정
- `제거`: 제거된 기능
- `알려진 사항`: 사용 전 알아야 할 제한 또는 주의점
