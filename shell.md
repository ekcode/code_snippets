# 각종 명령어

### sudo time-out

값은 분단위이다. 0으로 설정하면 항상 패스워드를 물어본다.

sudo visudo

change

`Defaults     env_reset`

to

`Defaults     env_reset,timestamp_timeout=2`

### whence -v 

outputs the file containing the function definition.

### keytool

JRE에 등록된 CA 리스트 확인

`$JAVA_HOME/jre/lib/security ➜  keytool -list -keystore cacerts`

CA 추가

`$JAVA_HOME/jre/lib/security ➜  keytool -keystore cacerts -importcert -alias comodorsa -file comodorsa.cer`


### ncdu

디스크 사용량 확인

`du -sh *` 보다 빠르고 한눈에 들어온다.


### lsof -n -i :3000

3000번 포트를 사용 중인 PID
