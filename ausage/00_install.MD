# 주의
- github은 수동으로 사용(수정후 항상 _git_push.bat)
- (주의)nred에서 프로젝트 사용하지 말 것
- (주의)프로젝트 생성시 각 프로젝트별로 .git가 생성됨 - 즉 flow버젼관리 >>> 프로젝트별로 git repo만들어야 함(맨아래참조)
- 


# bat
- _git_init.bat <<< 처음 git 생성시에만
- _git_push.bat <<< 수정시
- _start_nred.bat <<< 실행



# clone
- git clone https://github.com/algorik5/util-nred-aproject.git
- cd util-nred-aproject
- _start_nred.bat



# =============  node-red
npm install node-red -g <<< node_module아래에 설치됨
설정 - settings.js < node_module/node-red/settings.js복사 > nred_settings.js 
	port변경
	flowFilePretty: true
	projects/enabled=true
=== node-red-contrib-natsio 설치 - hello1/node_modules아래에 설치되는군... 흠....

# ============== node-red git project 사용법
1. github --- repo 생성 (ztest100)
2. nred --- 설정 > Git설정 > ssh키생성(testtest) > pubkey복사
	github --- settings/deploykeys에 add new,allow write
3. nred - 프로젝트 - 열기
	(ssh) git@github.com:algorik5/ztest100.git
	ssh키(testest),pass입력
	복제 > create default > 암호활성 > 커스텀키(testtest)
4. 소스수정
	 프로젝트이력 > 스테이징 > 커밋 > 커밋이력에서 push

