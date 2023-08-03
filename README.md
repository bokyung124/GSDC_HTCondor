# GSDC_HTCondor
2023 GSDC 데이터 컴퓨팅 스쿨

1. submit 역할의 서버에 접속하여 구성을 시작합니다.

2. 사전 환경설정
   * git 설치 및 ansible 환경을 구성하기 위한 코드를 다운로드 받습니다.
   ```bash
   sudo yum install -y epel-release
   sudo yum install -y git ansible
   ```

3. 실습코드를 다운로드 받습니다.
   ```bash
   git clone https://github.com/geonmo/GSDCSChool_HTCondor.git
   ```

4. 본인의 조별 숫자로 ansible 세팅 작업을 수행합니다. 
   ```bash
   ./group_setting.sh 
   ```
 
5. 모든 서버에 접속하여 계정을 생성하고 패스워드를 지정합니다.
   ```bash
   ssh nodeY.gX
   useradd -m -G wheel -u [UID] [ACCOUNT]
   passwd [ACCOUNT]
   ```
