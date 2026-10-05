# git 실습 저장소

Gitflow 흐름(브랜치 → PR → Merge)을 연습한 저장소입니다.

## 진행 상황

feature/zero → feature/mul → feature/div 순서로 브랜치를 옮겨가며 작업했습니다.
그 과정에서 feature/div 브랜치에 lib/zero.py, lib/mul.py 가 삭제되었고,
merge 이후 develop 에서도 두 파일이 빠져 있는 상태가 되었습니다.

## 해결

develop 에서 feature/restore 브랜치를 따서 누락된 두 파일을 복구한 뒤,
PR & Merge 로 develop 에 반영했습니다.

## 구조

lib/
├─ zero.py   # 0 반환
├─ mul.py    # 곱셈
└─ div.py    # 나눗셈
