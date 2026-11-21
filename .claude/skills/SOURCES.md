# 설치된 외부 스킬 출처

원본 저장소에서 복사했습니다. 데모 이미지·오디오, 렌더링된 예제 HTML, 테스트 폴더는 제외했습니다.

| 스킬 폴더 | 원본 저장소 | 커밋 |
|---|---|---|
| karpathy-guidelines | https://github.com/multica-ai/andrej-karpathy-skills | 2c60614 |
| banner-design,brand,design,design-system,slides,ui-styling,ui-ux-pro-max | https://github.com/nextlevelbuilder/ui-ux-pro-max-skill | 2de1134 |
| graphify | https://github.com/Graphify-Labs/graphify | b582ad4 |
| caveman | https://github.com/JuliusBrussee/caveman | a192894 |
| archify | https://github.com/tt-a1i/archify | 4478129 |
| humanizer | https://github.com/blader/humanizer | a32f244 |
| last30days | https://github.com/mvanhorn/last30days-skill | bb2f1ed |
| hallmark | https://github.com/Nutlope/hallmark | 04977e1 |
| frontend-slides | https://github.com/zarazhangrui/frontend-slides | 9906a34 |
| brainstorming,diagnosing-superpowers,dispatching-parallel-agents,executing-plans,finishing-a-development-branch,receiving-code-review,requesting-code-review,subagent-driven-development,systematic-debugging,test-driven-development,using-git-worktrees,using-superpowers,verification-before-completion,writing-plans,writing-skills | https://github.com/obra/superpowers | 22f0b46 |
| skill-inspector | https://github.com/NVIDIA/SkillSpector | 48e0f94 |
| ask-matt,codebase-design,diagnosing-bugs,domain-modeling,git-guardrails-claude-code,grill-me,grill-with-docs,grilling,handoff,implement,implement-spec,improve-codebase-architecture,pr,prototype,research,retro,setup-matt-pocock-skills,setup-pre-commit,tdd,teach,to-questionnaire,to-spec,to-tickets,triage,wait-what,wayfinder,wizard,writing-for-agents | https://github.com/mattpocock/skills | abeeaf9 |
| security-audit | https://github.com/cloudflare/security-audit-skill | c1c8a8c |
| planning-with-files | https://github.com/OthmanAdi/planning-with-files | c37abd7 |
| i-have-adhd | https://github.com/ayghri/i-have-adhd | 1ecea19 |
| canvas-design,slack-gif-creator,academy-guide,web-artifacts-builder,mcp-builder,discernment-nudge,algorithmic-art,webapp-testing,internal-comms,brand-guidelines,theme-factory,frontend-design,doc-coauthoring | https://github.com/anthropics/skills | e4bb5d9 |

2차 설치분은 NVIDIA SkillSpector(정적 분석, --no-llm)로 검사했습니다. 점수가 높게 나온 항목은 직접 확인한 결과 오탐이었습니다(임시 파일 삭제, 자체 스크립트 실행, 문서 속 보안 권고 문장).
mattpocock/skills의 code-review는 내장 /code-review와 이름이 같아 제외했습니다. in-progress 스킬도 제외했습니다.
anthropics/skills의 docx, xlsx, pptx, pdf, skill-creator, claude-api는 이미 내장되어 있어 제외했습니다.

## 중복 정리 (superpowers 기준으로 통일)

삭제한 스킬: tdd, diagnosing-bugs, grill-me, implement, implement-spec, writing-for-agents (superpowers 또는 다른 스킬과 중복), brand-guidelines (Anthropic 브랜드 전용), slides (design, frontend-slides와 중복), academy-guide (매 응답마다 실행됨), ask-matt, retro (삭제한 스킬에 의존).
추가 삭제: caveman (i-have-adhd와 답변 스타일이 겹침).
