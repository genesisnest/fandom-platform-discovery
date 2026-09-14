# fandom-platform-discovery

Fandom 플랫폼 서비스의 **Discovery — 서비스 이해와 기술 탐색** 단계 문서 저장소입니다.

- 상태: 계획
- 기간: 기획 분석 기간 2~3주
- 기준 자료: `요구사항_v1.00.xlsx`, FE기술검토 참고 (팀 공유 경로에 별도 보관 — 링크는 확정되면 이 문서에 추가합니다)

## 목표

- 기획이 아직 구체화되지 않은 상태에서 서비스의 공통 이해를 만든다.
- 이후 기능 개발에 넓게 영향을 주는 Frontend 방식을 작은 코드로 확인한다.
- 이번 Discovery에서는 DM, 라운지, 라이브, 쇼핑 기능을 완성하지 않는다. 가짜 데이터와 단순 권한으로 기술 흐름만 확인한다.

## 플랫폼 용어

| 표현 | 이 문서에서 뜻하는 범위 |
| --- | --- |
| 브라우저 웹 | Chrome, Safari 등 브라우저에서 여는 서비스. 데스크톱 웹과 모바일 브라우저 웹을 포함한다. |
| 모바일 브라우저 웹 | 휴대폰 브라우저에서 여는 웹. 필요하면 화면 폭이나 기능 범위를 따로 적는다. |
| WebView | Flutter 앱 안에서 웹 화면을 표시하는 방식. 브라우저 웹 코드를 재사용할 수 있다. |
| Flutter 네이티브 화면 | Flutter가 직접 그리는 앱 화면. WebView 화면과 구분한다. |

## Discovery Track 00 — 서비스와 요구사항 이해

- **예상 소요**: 1일. 각자 담당 영역을 읽고 Story를 정리한 뒤, 당일 설명 시간에 함께 맞춘다.
- **목적**: 팀원 모두 같은 서비스 용어와 주요 사용자 흐름을 이해한다. Excel의 기능 목록을 읽는 데서 끝내지 않고, 사용자가 어떤 조건에서 무엇을 하는지 정리한다.

**권장 진행 방식**

1. 현재 HI& 서비스와 공개 화면 살펴보기
2. Excel 요구사항 읽기
3. Story 추출 도구로 담당 영역의 사용자 Story 뽑기
4. 모두 모여 오후 미팅에서 담당 Story 설명하기
5. Story를 함께 비교하고, 용어 차이와 모호한 내용 표시하기

**영역 배분**

- 개발자 한 명당 영역 1~2개를 맡는 방식을 권장한다.
- 각 영역에서 여러 사용자 Story를 뽑는다. 모든 기능을 빠짐없이 정리하는 일은 이번 범위에 넣지 않는다.

## 문서 작성 및 push 방법

Discovery 단계는 속도를 우선하므로 별도 브랜치/PR 없이 진행합니다.

```bash
git clone https://github.com/genesisnest/fandom-platform-discovery.git
cd fandom-platform-discovery
# docs/discovery/service-understanding/ 에 담당 영역 문서를 추가한 뒤
git add docs/discovery/service-understanding/<파일명>
git commit -m "Add <담당 영역> story notes"
git push origin main
```

파일 네이밍 규칙은 아직 정해지지 않았습니다. 팀 미팅에서 규칙을 확정하기 전까지는 자유로운 이름으로 문서를 추가해 주세요. 자세한 안내는 [`docs/discovery/service-understanding/README.md`](docs/discovery/service-understanding/README.md)를 참고하세요.

## 폴더 구조

```
docs/
  discovery/
    service-understanding/   # Track 00: 담당 영역별 Story 정리 문서
```
