# Template

```
.
├── AGENTS.md - 문서 체계, 반복되는 문제(핵심 라이브러리 버전 문제 등), 프로젝트 정의 등
├── CLAUDE.md - `AGENTS.md`를 가리킴
├── USAGE.md / README.md / PLAN.md / DESIGN.md - 필요에 따라 참고용으로 사용
├── adr - Architecture Decision Records
│   ├── <id>-json-schema-contract-between-analyzer-and-renderer.md - 실제 adr
│   ├── index.md - index 파일
│   └── stale.md - 폐기 표시
├── myTODO.md (.gitignore) - 프로젝트 관리용 노트
├── synced-comments
│   └── <synced_id>.md
└── ref
    ├── feats
    │   ├── <id>-multi-language-dependency-analyzers.md - 실제 feature
    │   ├── index.md - index 파일
    │   └── stale.md - 폐기 표시
    └── issues
        ├── <id>-kotlin-comment-string-literal-false-positive.md - 실제 issue
        ├── index.md - index 파일
        └── stale.md - 폐기 표시

```

Ready-to-go template for new project.

## synced-comment

`synced_id` is a random ID; its tracking file's `code_hash` is a hash of participating files' content except comments, concatenated in alphanumeric order of filenames, used to detect when the code drifts from the documented comment. Change this as your team needs. But I actually recommend to keep your files small and modular