# ✦ AX 컨퍼런스 트래커

> AI·신기술 컨퍼런스·세미나 자동 수집 에이전트  
> 운영자: leema1206 · 주소: https://leema1206.github.io/ax-tracker

---

## 📁 파일 구성

```
ax-tracker/
├── index.html    ← 메인 앱 (이것만 있으면 됩니다)
├── data.json     ← 백업용 데이터 저장소
└── README.md     ← 이 파일
```

---

## 🚀 GitHub Pages 배포 방법 (최초 1회)

### 1단계 · Repository 만들기
1. [github.com/new](https://github.com/new) 접속
2. Repository name: **`ax-tracker`** 입력
3. **Public** 선택 (GitHub Pages 무료 사용 조건)
4. **Create repository** 클릭

### 2단계 · 파일 올리기
1. 방금 만든 repository 페이지에서 **"uploading an existing file"** 클릭
2. `index.html`, `data.json`, `README.md` 세 파일을 드래그앤드롭
3. 아래 **Commit changes** 클릭

### 3단계 · GitHub Pages 활성화
1. Repository → **Settings** 탭
2. 왼쪽 메뉴 **Pages** 클릭
3. Source: **Deploy from a branch**
4. Branch: **main** / `/ (root)` 선택 → **Save**
5. 1~2분 후 `https://leema1206.github.io/ax-tracker` 접속 가능!

---

## 💾 데이터 히스토리 보존 방법

이 앱은 브라우저 localStorage에 데이터를 저장합니다.  
**영구 보존을 위해 주기적으로 아래 절차를 따라주세요:**

### 매주 수집 후
1. 앱에서 **"JSON 백업"** 버튼 클릭 → `ax_tracker_backup_날짜.json` 다운로드
2. GitHub repository에서 **Add file → Upload files**
3. 다운받은 JSON 파일을 `data.json`으로 이름 바꿔서 업로드
4. Commit → 완료!

> 이렇게 하면 어떤 기기에서 접속해도 JSON 불러오기로 히스토리 복원 가능

---

## 📋 주요 기능

| 기능 | 설명 |
|------|------|
| 🔍 자동 수집 | Claude AI가 웹 검색으로 행사 정보 수집 |
| 📋 대시보드 | 가까운 행사 카드뷰로 표시 |
| 📝 전체 목록 | 필터·검색·정렬 |
| 📅 수집 히스토리 | 언제 몇 건 수집했는지 기록 |
| ⚙ 양식 편집 | 수집 항목 추가/삭제/변경 |
| + 직접 추가 | 수동으로 행사 입력 |
| 📥 CSV 저장 | 엑셀에서 열 수 있는 파일 |
| 💾 JSON 백업 | 전체 데이터 백업 |
| 📂 JSON 불러오기 | 백업 파일로 복원 |

---

## ❓ 자주 묻는 질문

**Q. 데이터가 사라졌어요**  
A. JSON 백업 파일이 있다면 "JSON 불러오기" 버튼으로 복원하세요.

**Q. 실제로 웹 검색이 되나요?**  
A. Claude API 키 설정이 필요합니다. 없으면 샘플 데이터로 동작합니다.

**Q. 다른 사람과 공유하고 싶어요**  
A. `leema1206.github.io/ax-tracker` URL을 공유하면 됩니다. (읽기 전용)
