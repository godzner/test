pip3 install django~=2.1.0
python3 manage.py runserver 0.0.0.0:80
goo.gl/88dgrN

sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv --keyserver packages.microsoft.com --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF

설치 후

az

az login

az webapp list

az webapp up --name msdevops20190312002 --location "Korea Central"

az group delete -n msdevops20190312002

1. Azure Portal
   * Azure Portal에서 웹앱의 Deployment Center에 가셔서 Local Git으로 배포방법을 변경
   * 같은 페이지에서 clone url을 복사해두시고, 상단의 credential 버튼을 통해 유저명/암호 정보를 획득합니다.
2. 구름 IDE : git remote 주소로서 origin 등록
   * 쉘> git remote add origin 복사한_주소
   * 배포 진행 : 쉘> git push origin master
3. 구름 IDE
   * 프로젝트/urls.py 에 root 뷰 구현하시고
   * 커밋 : 쉘> git commit -a -m "root 뷰 구현"
   * 배포 수행 : 쉘> git push origin master

# 구름 IDE의 git 저장소에서
git remote add origin 복사한_주소
git push origin master # 실제 설치과정들이 표준출력으로 보여짐.
 - 유저명/암호 인증을 요구

추가로 개발하고 커밋한 후에, 언제라도 배포를 원할 때 git push origin master 를 하시면 됩니다,

슬롯 기능 : 웹앱을 복제하여 테스트 후 서비스 중지 없이 스왑 가능
