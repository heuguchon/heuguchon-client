# Firestorm 뷰어 한글화 작업 계획

## 프로젝트 개요
- **대상**: SecondLife Firestorm 뷰어
- **목표**: 한국어 번역 추가
- **언어 코드**: ko (한국어)
- **작업 위치**: `indra/newview/skins/default/xui/ko/`

## 작업 현황 파악

### 언어 파일 구조
1. **영어(en) 파일**: `xui/` 루트에 위치, 완전한 UI 정보 포함
2. **다른 언어 파일**: 각 언어별 폴더에 위치, i18n 번역 정보만 포함
   - `xui/az/` (아제르바이잔어)
   - `xui/da/` (덴마크어) 
   - `xui/de/` (독일어)

### 번역 대상 요소
- `label` 속성: UI 텍스트 라벨
- `tool_tip` 속성: 툴팁 텍스트
- `name` 속성 (일부): 이름 필드

## 작업 계획

### 1단계: 환경 준비 ✅
- [x] 프로젝트 구조 파악
- [x] 기존 번역 언어 확인 (az, da, de)
- [x] 작업 계획 문서 생성

### 2단계: 한국어 폴더 생성 ✅
- [x] `xui/ko/` 디렉토리 생성
- [x] 기본 구조 파악 및 샘플 파일 분석

### 3단계: 파일 우선순위 설정 ✅
- [x] 핵심 UI 파일 식별 (메뉴, 기본 대화상자 등)
- [x] 번역 우선순위 순서 결정

### 4단계: 번역 작업 🎯
- [x] 1차: 핵심 파일 번역 시작
  - [x] strings.xml (기본 문자열)
  - [x] floater_about.xml (정보 창)
  - [x] menu_login.xml (로그인 메뉴)
- [x] 2차: 주요 플로터(Floater) 창 번역
  - [x] floater_preferences.xml (환경설정)
  - [x] floater_my_inventory.xml (인벤토리)
  - [x] floater_world_map.xml (지도)
  - [x] floater_fs_search.xml (검색)
  - [x] floater_fs_nearby_chat.xml (근처 채팅)
  - [x] floater_fs_im_container.xml (IM 컨테이너)
  - [x] floater_people.xml (사람 목록)
  - [x] floater_my_appearance.xml (외모 편집)
  - [x] floater_places.xml (장소)
  - [x] language_settings.xml (언어 설정)
- [x] 3차: 주요 메뉴 번역
  - [x] menu_edit.xml (편집 메뉴)
  - [x] menu_inventory.xml (인벤토리 메뉴)
  - [x] menu_object.xml (객체 컨텍스트 메뉴)
  - [x] menu_land.xml (토지 컨텍스트 메뉴)
  - [x] menu_avatar_other.xml (다른 사용자 메뉴)
  - [x] menu_avatar_self.xml (자신 메뉴)
- [ ] 4차: 기타 UI 요소

### 5단계: 검증 및 최적화
- [ ] 번역 품질 확인
- [ ] UI 레이아웃 호환성 검증
- [ ] 문자 인코딩 확인

## 참조할 파일 예시

### 독일어(de) 파일 수
약 400여개의 XML 파일이 번역되어 있음

### 주요 파일 카테고리
1. **floater_*.xml**: 독립적인 창 UI
2. **menu_*.xml**: 메뉴 시스템
3. **panel_*.xml**: 패널 UI
4. **strings.xml**: 일반 문자열
5. **notifications.xml**: 알림 메시지

## 작업 진행 상황

### 완료된 작업
- 프로젝트 구조 분석
- 작업 계획 수립
- ko 폴더 생성
- **핵심 파일 19개 번역 완료:**
  - strings.xml (기본 문자열)
  - floater_about.xml (정보 창)
  - menu_login.xml (로그인 메뉴)
  - floater_preferences.xml (환경설정)
  - floater_my_inventory.xml (인벤토리)
  - floater_world_map.xml (지도)
  - floater_fs_search.xml (검색)
  - floater_fs_nearby_chat.xml (근처 채팅)
  - floater_fs_im_container.xml (IM 컨테이너)
  - floater_people.xml (사람 목록)
  - floater_my_appearance.xml (외모 편집)
  - floater_places.xml (장소)
  - language_settings.xml (언어 설정)
  - menu_edit.xml (편집 메뉴)
  - menu_inventory.xml (인벤토리 메뉴)
  - menu_object.xml (객체 컨텍스트 메뉴)
  - menu_land.xml (토지 컨텍스트 메뉴)
  - menu_avatar_other.xml (다른 사용자 메뉴)
  - menu_avatar_self.xml (자신 메뉴)

### 진행 중인 작업
- 추가 중요 UI 파일 식별 및 번역

### 다음 단계
1. 메인 뷰어 메뉴 파일 번역 (menu_viewer.xml - 대용량)
2. 채팅 관련 UI 파일들 번역
3. 알림(notifications.xml) 시스템 번역 (대용량)
4. 패널 UI 요소들 번역

---

*작업 시작일: 2025-08-14*
*최종 수정일: 2025-08-14*

## 작업 요약

### 오늘 수행한 작업 (2025-08-14)
- 프로젝트 구조 분석 및 ko 폴더 생성
- **19개 핵심 UI 파일 번역 완료**
- 기본 로그인, 메뉴, 채팅, 지도, 검색 등 핵심 기능 포함
- 언어 설정 파일로 한국어 로케일 지원
- **주요 컨텍스트 메뉴 번역 완료** (객체, 토지, 아바타 메뉴)

### 다음 단계 우선순위
1. **대용량 파일 번역**:
   - menu_viewer.xml (48KB) - 메인 뷰어 메뉴
   - floater_tools.xml (27KB) - 빌드 도구
   - notifications.xml (288KB) - 알림 시스템

2. **추가 핵심 기능 파일들**:
   - 지역 및 언어 관련 파일들
   - 오류 메시지 및 도움말 파일들
   - 패널 UI 요소들

3. **검증 및 최적화**:
   - 번역 품질 확인
   - UI 레이아웃 호환성 검증
   - 한글 인코딩 확인