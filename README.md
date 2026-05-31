# 🧰 FileKit

과제 제출 전 필요한 모든 파일 작업을 **한 곳에서, 서버 없이, 브라우저에서** 처리하는 올인원 파일 도구입니다.

모든 처리가 사용자의 브라우저 안에서만 이루어지므로 파일이 외부 서버로 전송되지 않습니다. (개인정보·보안 안전)

## ✨ 기능

| 기능 | 설명 |
|------|------|
| 🗜️ **압축** | 이미지·PDF·DOCX를 종류에 맞게 압축. 비슷한 이름끼리 자동 그룹핑 |
| 🔄 **변환** | 이미지 ↔ JPG/PNG/WebP/PDF, PDF → PNG 이미지 |
| 📋 **글자 추출** | 이미지 OCR(한국어+영어), PDF·DOCX 본문 텍스트 추출 → 복사·txt 저장 |
| 🔗 **PDF 합치기** | 여러 PDF를 원하는 순서대로 하나로 병합 |
| 📑 **제출 검사** | 제출 전 PDF 자동 점검 (용량·페이지 수·빈 페이지·가로 페이지) |
| 📦 **압축팩** | `학번_이름_과제.zip` 형식으로 자동 정리·압축 |
| 🔍 **중복 탐지** | 내용이 같거나(SHA-256) 이름이 비슷한 중복 파일 탐지 |
| 🍎 **HEIC 변환** | 아이폰·맥 사진(HEIC/HEIF) → JPG |

그 외: 🎨 글래스모피즘 디자인 · 라이트/다크 모드 · 드래그앤드롭 · 전체 진행률 표시

## 🛠️ 기술 스택

- HTML + Vanilla JavaScript + CSS (단일 파일, 빌드 불필요)
- [JSZip](https://stuk.github.io/jszip/) — ZIP 생성·해제
- [pdf-lib](https://pdf-lib.js.org/) — PDF 합치기·압축·생성
- [pdf.js](https://mozilla.github.io/pdf.js/) — PDF 렌더링·텍스트 추출
- [Tesseract.js](https://tesseract.projectnaptha.com/) — OCR
- [heic2any](https://github.com/alexcorvi/heic2any) — HEIC 변환

## 🚀 실행

별도 빌드 없이 `index.html`을 브라우저로 열면 됩니다.

```bash
https://filekit-seven.vercel.app
```

## 📦 배포

Vercel 정적 호스팅으로 배포되었습니다.
