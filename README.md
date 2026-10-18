# 3톡 (3TOK) v2.1 — Windows 무료 프로그램

> ⬇️ **다운로드: [Releases 페이지](../../releases/latest)** 에서 `3TOK-v2.1-win-x64.zip` 을 받으세요.
> 이 저장소에는 프로그램 소스가 없고, 안내 문서와 배포 파일의 검증 정보만 있어요.

**나(1토커)와 두 AI(2토커·3토커)가 함께 대답하고, 논의하고, 회의하는 개인용 프로그램이에요.**

제작: **유리나무yuriwood** · 무료 프리웨어 · Copyright (c) 2026 유리나무yuriwood

- ChatGPT·Claude·Gemini 중 원하는 두 AI를 골라 써요. (내 API 키가 필요해요)
- Node.js 같은 개발 도구 없이 **압축을 풀고 `3TOK.exe`를 더블클릭**하면 돼요.
- 대화 기록과 API 키는 내 컴퓨터(`%APPDATA%\3TOK`)에만 저장돼요. 제작자에게 아무것도 전송하지 않아요.

## 빠른 시작
1. `3TOK-v2.1-win-x64.zip` 압축 해제
2. `3TOK.exe` 더블클릭 (처음에 Windows 경고가 나오면 **추가 정보 → 실행**)
3. 열린 화면 위쪽 **[토커 설정]** 에서 내 API 키 입력 → **연결됨** 확인
   (브라우저가 안 열리면 검은 창에 출력된 `http://localhost:3000/#k=…` 전체 주소를 복사해 붙여 넣어요.)
4. 2토커·3토커 AI를 고르고 질문하기

자세한 사용법은 **[USER_GUIDE.md](USER_GUIDE.md)** 를 보세요.

## 포함된 파일
| 파일 | 설명 |
|---|---|
| `3TOK.exe` | 프로그램 (단일 실행 파일, Windows 10/11 64비트) |
| `USER_GUIDE.md` | 사용 설명서 |
| `LICENSE.txt` | 이용허락서 (무료 사용, 재배포 조건) |
| `THIRD_PARTY_NOTICES.txt` | 포함된 오픈소스(Node.js, Pretendard)의 라이선스 고지 |
| `SECURITY_AUDIT.md` | 보안 검수 보고서 |
| (릴리스 페이지의 `SHA256SUMS.txt`) | ZIP과 `3TOK.exe`의 무결성 확인용 해시. ZIP 안에는 들어 있지 않고 다운로드 페이지에 함께 올라가요. ZIP 줄은 압축을 풀기 전에, `3TOK.exe` 줄은 압축을 푼 뒤에 확인해요. `3TOK.exe` 해시는 `SECURITY_AUDIT.md`에도 적혀 있어요. |
| `Create-Desktop-Shortcut.cmd` | (선택) 바탕화면 바로가기 만들기 |

## 꼭 알아두세요
- **API 사용료**는 각 AI 회사가 쓴 만큼 따로 청구해요. ChatGPT Plus·Claude Pro 같은 월 구독과는 별개예요. 결제 한도를 꼭 걸어 두세요.
- 이 프로그램은 코드 서명이 되어 있지 않아 처음 실행 시 Windows SmartScreen 경고가 나올 수 있어요.
- 프로그램은 `127.0.0.1`(내 컴퓨터)에서만 열려요. 내가 질문하거나 [토커 설정]·연결 테스트를 쓸 때만 OpenAI·Anthropic·Google API 주소로 접속해요. 프로그램을 켤 때는 접속하지 않아요.

## 파일이 진짜인지 확인
```
Get-FileHash .\3TOK.exe -Algorithm SHA256
```
릴리스 페이지의 `SHA256SUMS.txt`(또는 `SECURITY_AUDIT.md`)에 적힌 `3TOK.exe` 값과 같아야 해요.
