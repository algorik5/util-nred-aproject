


# ============= (참고) node-red 시작하기
- npm install node-red -g <<< node_module아래에 설치됨
- 설정 - settings.js < node_module/node-red/settings.js복사 > nred_settings.js 
  - port변경
  - flowFilePretty: true
  - flowFile: 'flows.json'
  - projects/enabled=true
- === node-red-contrib-natsio 설치 - hello1/node_modules아래에 설치되는군... 흠....


# ============== (주의) nred project 사용하기 (projects/enabled=true)
- (주의)nred에서 프로젝트 사용하지 말 것
- (주의)프로젝트 생성시 각 프로젝트별로 .git가 생성됨 - 즉 flow별 버젼관리를 의미 >>> 프로젝트별로 git repo만들어야 함(nred_install.MD 참고)
# ====  (참고) node-red git project 사용법
- (참고-동영상) https://www.youtube.com/watch?v=Bto2rz7bY3g
- 1. github --- repo 생성 (ztest100)
- 2. nred --- 설정 > Git설정 > ssh키생성(testtest) > pubkey복사
  - github --- settings/deploykeys에 add new,allow write
- 3. nred - 프로젝트 - 열기
  - (ssh) git@github.com:algorik5/ztest100.git
  - ssh키(testest),pass입력
  - 복제 > create default > 암호활성 > 커스텀키(testtest)
- 4. 소스수정
  - 프로젝트이력 > 스테이징 > 커밋 > 커밋이력에서 push

