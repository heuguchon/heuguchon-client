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

### 4단계: 번역 작업 🚀
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
- [x] 4차: 추가 중요 플로터 번역
  - [x] floater_camera.xml (카메라 컨트롤)
  - [x] floater_gesture.xml (제스처)
  - [x] floater_snapshot.xml (스크린샷)
  - [x] floater_pay.xml (지불)
  - [x] floater_sound_devices.xml (사운드 장치)
  - [x] floater_stats.xml (통계)
- [x] 5차: 1단계 추가 중요 플로터 번역 완료
  - [x] floater_profile.xml (프로필 창)
  - [x] floater_fs_group.xml (그룹 관리)
  - [x] floater_im_session.xml (IM 세션)
  - [x] floater_how_to.xml (도움말)
  - [x] floater_script_debug.xml (스크립트 디버그)
- [x] 6차: 2단계 추가 중요 플로터 번역 완료
  - [x] floater_build_options.xml (건축 옵션)
  - [x] floater_avatar_picker.xml (아바타 선택기)
  - [x] floater_help_browser.xml (도움말 브라우저)
  - [x] floater_media_browser.xml (미디어 브라우저)
  - [x] floater_buy_currency.xml (통화 구매)
- [x] 7차: 추가 플로터 창 번역 완료 (6개)
  - [x] floater_region_info.xml (지역/부동산 정보)
  - [x] floater_auction.xml (린든 토지 판매)
  - [x] floater_bulk_perms.xml (대량 권한 설정)
  - [x] floater_fs_radar.xml (레이더)
  - [x] floater_inspect.xml (객체 검사)
  - [x] floater_web_content.xml (웹 콘텐츠)
- [x] 8차: Option B 추가 플로터 창 번역 완료 (3개)
  - [x] floater_buy_land.xml (토지 구매)
  - [x] floater_search.xml (검색 시스템)
  - [x] floater_inventory_item_properties.xml (아이템 속성)
- [x] 9차: 1차 채팅/커뮤니케이션 관련 완료 (3개)
  - [x] floater_conversation_log.xml (대화 기록)
  - [x] floater_voice_chat_volume.xml (음성 채팅 볼륨)
  - [x] floater_voice_effect.xml (음성 변조 미리보기)
- [x] 10차: 2차 빌드/편집 도구 관련 완료 (3개)
  - [x] floater_object_weights.xml (객체 무게 정보)
  - [x] floater_particle_editor.xml (파티클 에디터)
  - [x] floater_openobject.xml (객체 열기)
- [x] 11차: 3차 인벤토리/아이템 관리 관련 완료 (3개)
  - [x] floater_inventory_settings.xml (인벤토리 설정)
  - [x] floater_outfit_save_as.xml (의상 저장)
  - [x] floater_inventory_view_finder.xml (인벤토리 검색)
- [ ] 12차: 대용량 파일 도전 (menu_viewer.xml, notifications.xml 등)
- [ ] 6차: 기타 UI 요소

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
- **핵심 파일 44개 번역 완료:**
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
  - floater_camera.xml (카메라 컨트롤)
  - floater_gesture.xml (제스처)
  - floater_snapshot.xml (스크린샷)
  - floater_pay.xml (지불)
  - floater_sound_devices.xml (사운드 장치)
  - floater_stats.xml (통계)
  - floater_profile.xml (프로필 창)
  - floater_fs_group.xml (그룹 관리)
  - floater_im_session.xml (IM 세션)
  - floater_how_to.xml (도움말)
  - floater_script_debug.xml (스크립트 디버그)
  - floater_build_options.xml (건축 옵션)
  - floater_avatar_picker.xml (아바타 선택기)
  - floater_help_browser.xml (도움말 브라우저)
  - floater_media_browser.xml (미디어 브라우저)
  - floater_buy_currency.xml (통화 구매)
  - floater_region_info.xml (지역/부동산 정보)
  - floater_auction.xml (린든 토지 판매)
  - floater_bulk_perms.xml (대량 권한 설정)
  - floater_fs_radar.xml (레이더)
  - floater_inspect.xml (객체 검사)
  - floater_web_content.xml (웹 콘텐츠)
  - floater_buy_land.xml (토지 구매)
  - floater_search.xml (검색 시스템)
  - floater_inventory_item_properties.xml (아이템 속성)
  - floater_conversation_log.xml (대화 기록)
  - floater_voice_chat_volume.xml (음성 채팅 볼륨)
  - floater_voice_effect.xml (음성 변조 미리보기)
  - floater_object_weights.xml (객체 무게 정보)
  - floater_particle_editor.xml (파티클 에디터)
  - floater_openobject.xml (객체 열기)
  - floater_inventory_settings.xml (인벤토리 설정)
  - floater_outfit_save_as.xml (의상 저장)
  - floater_inventory_view_finder.xml (인벤토리 검색)

### 진행 중인 작업
- 추가 중요 UI 파일 식별 및 번역

### 다음 단계
1. 더 많은 플로터 창 번역 (채팅, 그룹, 프로필 관련)
2. 메인 뷰어 메뉴 파일 번역 (menu_viewer.xml - 대용량)
3. 알림(notifications.xml) 시스템 번역 (대용량)
4. 패널 UI 요소들 번역

---

*작업 시작일: 2025-08-14*
*최종 수정일: 2025-08-14*

## 작업 요약

### 오늘 수행한 작업 (2025-08-14)
- 프로젝트 구조 분석 및 ko 폴더 생성
- **53개 핵심 UI 파일 번역 완료**
- 기본 로그인, 메뉴, 채팅, 지도, 검색 등 핵심 기능 포함
- 언어 설정 파일로 한국어 로케일 지원
- **주요 컨텍스트 메뉴 번역 완료** (객체, 토지, 아바타 메뉴)
- **핵심 플로터 창들 번역 완료** (카메라, 제스처, 스크린샷, 지불, 통계 등)
- **추가 중요 UI 번역 완료** (프로필, 그룹, IM 세션, 도움말, 스크립트 디버그)
- **2단계 고급 UI 번역 완료** (건축, 아바타 선택, 도움말 브라우저, 미디어 브라우저, L$ 구매)
- **3단계 고급 번역 완료** (지역 정보, 경매, 권한 설정, 레이더, 객체 검사, 웹 콘텐츠)
- **Option B 추가 번역 완료** (토지 구매, 검색 시스템, 아이템 속성)
- **1차 채팅/커뮤니케이션 번역 완료** (대화 기록, 음성 채팅 볼륨, 음성 변조)
- **2차 빌드/편집 도구 번역 완료** (객체 무게, 파티클 에디터, 객체 열기)
- **3차 인벤토리/아이템 관리 번역 완료** (인벤토리 설정, 의상 저장, 인벤토리 검색)

### 번역 완료율
- **총 53개 파일 번역** (독일어 기준 약 400개 중 약 13%)
- **핵심 사용자 인터페이스 완료** - 기본적인 SecondLife 사용에 충분
- **메뉴 시스템 완료** - 대부분의 메뉴 및 컨텍스트 메뉴 한국어화

### 다음 단계 우선순위
1. **더 많은 플로터 창들**:
   - 그룹 관리 (floater_fs_group.xml 등)
   - 프로필 관련 (floater_profile.xml 등)
   - 빌드/편집 도구들
   - 채팅 관련 추가 파일들

2. **대용량 파일 도전**:
   - menu_viewer.xml (48KB) - 메인 뷰어 메뉴
   - floater_tools.xml (27KB) - 빌드 도구
   - notifications.xml (288KB) - 모든 알림 메시지

3. **검증 및 최적화**:
   - 번역 품질 확인
   - UI 레이아웃 호환성 검증
   - 한글 인코딩 확인