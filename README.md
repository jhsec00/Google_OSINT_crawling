# Google_OSINT_crawling
구글 site url 수집기


Google `site:` 검색 결과를 자동으로 수집하여  
**제목 / URL / 스니펫 / 페이지 정보**를 엑셀로 저장하는 OSINT(Open Source Intelligence) 목적의 크롤러입니다.

---

## ✨ 주요 기능

- Google `site:도메인` 검색 자동화
- 검색 결과 **Title / URL / Snippet** 수집
- **다음 버튼이 없어질 때까지 자동 페이지네이션**
- Headless 모드 (브라우저 화면 미표시)
- 이미지 로딩 차단으로 속도 향상
- 중간 종료(Ctrl+C, 오류) 시에도 결과 자동 저장
- Excel 자동 생성
  - 날짜·시간 포함 파일명
  - 자동 테두리
  - 자동 열 너비 조정

---

## 📊 출력 엑셀 컬럼

| 컬럼명 | 설명 |
|------|------|
| idx | 순번 |
| 제목 | Google 검색 결과 제목 |
| url | 접근 URL |
| 내용 | 검색 결과 스니펫 |
| page | 검색 결과 페이지 번호 |
| 비고 | 사용자 메모 |

---

## 📦 설치 방법

```bash
pip install -r requirements.txt
```

## 🚀 사용 예시

```bash
python run.py -t example.com --min-delay 1 --max-delay 3
```
