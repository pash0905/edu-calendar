# 교육일정 관리 웹앱 v2

##계정
- GitHub 및 Supabase 접속계정은 pasuhw0905@google.com 
- Supabase edu_calendar 프로젝트 비번은 'kd#5050one@'

## 반영사항
- 대한민국 공휴일 자동 표시
- GitHub Pages 정적 호스팅 + Supabase DB 연동 구조
- 일정 1건 = DB 1행 구조로 정규화
- 교육명/담당자/장소/구분/색상/메모 관리
- 월 이동, 월 선택, 4/5/6주 자동 달력
- Excel/CSV 다운로드

## 사용 순서
1. Supabase에서 새 프로젝트 생성
2. SQL Editor에서 supabase_schema.sql 실행
3. seed_events.sql 실행
4. config.js의 SUPABASE_URL, SUPABASE_ANON_KEY를 입력하고 USE_SUPABASE를 true로 변경
5. GitHub 저장소에 index.html, config.js, initial_events.json 업로드
6. Settings > Pages에서 배포

## 주의
supabase_schema.sql은 MVP용 공개 정책입니다. 웹주소를 아는 사람이 모두 수정할 수 있습니다. 회사 내부 운영용은 로그인/Auth 권한관리로 확장하세요.
