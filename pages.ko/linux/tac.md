# tac

> 파일의 내용을 역순으로 표시하고 연결합니다.
> 같이 보기: `cat`.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/manual/html_node/tac-invocation.html>.

- 특정 파일들을 역순으로 연결:

`tac {{경로/대상/파일1 경로/대상/파일2 ...}}`

- `stdin`을 역순으로 표시:

`{{cat 경로/대상/파일}} | tac`

- 특정 구분자 사용:

`tac --separator {{,}} {{경로/대상/파일1 경로/대상/파일2 ...}}`

- 특정 정규식을 구분자로 사용:

`tac --regex --separator {{[,;]}} {{경로/대상/파일1 경로/대상/파일2 ...}}`

- 각 파일 앞에 구분자 사용:

`tac --before {{경로/대상/파일1 경로/대상/파일2 ...}}`
