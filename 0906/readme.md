이번 시간에는 0830 과정에서 더 나아가서 명령어 시작까지 해보도록 하겠습니다.

![10](https://github.com/user-attachments/assets/dcd56659-9b0b-4dd8-93b6-0432520dae21)

까지 진행되었으면 이제 여기서 wsl 을 입력해주시면 

아래 사진과 같이 나오게 되면서 로그인이 됩니다 (0830 과정을 거치면서 계정을 만든경우)

![11](https://github.com/user-attachments/assets/d9fd8cc5-19e6-45e7-a737-1d1d7f624900)

명령어를 입력하기 전에 현재의 디렉토리 위치를 보면
/mnt/c/Users/(사용자 이름) 으로 되있는걸 확인할수 있습니다.

여기서 cd 를 입력하여 주시면 
/mnt/c/Users/(사용자 이름) 이 없어진 것을 볼수 있습니다
이 상태에서 명령어인 pwd 를 입력하시면

![12](https://github.com/user-attachments/assets/16459565-f504-4c39-9646-51bd01ca9dd7)

사진과 같이 /home/(사용자이름) 이 결과로 나오는 것을 알 수 있습니다.

이제 다음부터 사용할 tree 라는 명령어를 사용하기 위해 0830 파일에서 했던
sudo apt upgrade, sudo apt update 를 입력해줍시다.
업데이트가 끝난 후에는 
sudo apt install tree 를 입력해서 설치해줍시다.

설치가 끝난 후에 tree를 입력하면 비어있는 것을 확인할수 있습니다.

![13](https://github.com/user-attachments/assets/a35afba2-b348-4d6e-9668-e8b322ad16a0)


tree 는 현재의 디렉토리에서 하위 디렉토리와, 파일들을 확인할수 있게해주는 명령어임으로
현재 사용하고 있는 위치인 /home/(사용자이름) 에는 아무것도 진행하지 않았기에 안나오는 것이 맞습니다.
