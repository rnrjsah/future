이번시간에는 wsl 설치를 한 것을 기준으로 합니다.

시작함에있어서 여러가지 명령어를 알아보고 시작을 해봅시다.

wsl 에는 네트워크 관련 명령어, 사용자 설정 명령어, 디렉토리 확인 명령어 등 많은 명령어들이 있습니다.
오늘 배울것을 제외하고 man {궁금한 명령어} 를 입력하면 어떤 명령어인지 어떤 옵션이 있는지 나오게 됩니다.

예시로 ls 에 대한 다양한 옵션들을 보고싶다면
아래 사진처럼

![20](https://github.com/user-attachments/assets/2f50e245-c597-4a77-8558-b4af1ae40613)

man ls 를 입력하고 Enter 키를 눌러주면

![21](https://github.com/user-attachments/assets/80591d20-364e-4f71-9c11-ed093ba499b8)


위 사진처럼 ls 명령어의 옵션, 사용방법이 나오게 됩니다.

여기서 나올때는 q 키를 눌러주면

![22](https://github.com/user-attachments/assets/5d441945-ada2-43fa-8fd4-4ebab573723c)

사진처럼 나와지게 됩니다.

처음으로 확인할 명령어들은 기초적인 명령어들만 해봅시다.
pwd, rmdir, mkdir, cd 명령어들을 간단하게 알아봅시다

cd는 디렉토리를 원하는 위치로 이동하는 명령어이다.
pwd는 현재의 디렉토리의 위치 확인하는 명령어이다.
mkdir는 파일의 생성하는 명령어이다.
rmdir는 디렉토리삭제를 하는 명령어이다.

위 명령어 사용예시를 보여드리겠습니다.
(사진에서 사용하는 트리는 sudo apt install tree 명령어를 입력하고 나면 사용가능합니다.)
우선 기본 환경에서 mkdir OS 를 입력해 OS 라는 디렉토리를 생성해줍니다.

![23](https://github.com/user-attachments/assets/303f5bb6-95fa-48ae-8abc-1c847b01a456)

다음으로는 cd OS 를 입력해 OS 디렉토리로 이동해줍시다.
그 후 mkdir Linux 를 입력해 Linux 디렉토리를 생성해주고 tree 를 입력하면 OS 하위 디렉토리인 Linux 가 있는걸 볼수 있습니다.

![24](https://github.com/user-attachments/assets/082a05ac-a32a-4b1b-8e7a-a2e41a89de4e)

이제 삭제하는 명령어를 사용해봅시다. 
rmdir OS 를 그냥 입력하면 아래 사진과 같은 메시지가 나오는데

![25](https://github.com/user-attachments/assets/14171892-5c96-41ee-a711-0c1b97abe8bb)

이 메시지는 OS 내부의 디렉토리가 비워지지않았기에 나오는 메시지입니다.
이에따라 cd OS 를 입력 해준다음 rmdir Linux, rmdir Windows 를 입력해주고
cd 를 입력한후 tree를 입력하면 아래 사진과 같은 결과가 나옵니다.

![26](https://github.com/user-attachments/assets/19efbaae-651f-4962-b800-cd070372075d)

이제 rmdir OS 를 해주면 디렉토리가 삭제됬음을 확인할수 있습니다.

![27](https://github.com/user-attachments/assets/9c11853b-100e-4762-9ab4-ecc78d5dfb1f)


그 다음 알아볼 명령어들은 
rm, mv, ls 명령어들 입니다.

rm는 파일 삭제를 해주는 명령어이며, 옵션으로 -r 을 하게되면 하위 파일들 역시도 삭제됩니다.(복구도 안되니 주의하며 사용합시다.)
mv는 파일의 이동을 해주는 명령어입니다.
ls 디렉토리 내의 파일을 확인하는 명령어입니다.

이 코드들 역시도 실습을 해봅시다.
우선 ls 먼저 확인을 하기위해 아래 사진과 같이 디렉토리 생성을 먼저 해줍시다.

![28](https://github.com/user-attachments/assets/38c9706e-aee6-4f59-afd6-a569f1c67ee6)

생성이 끝나면 디렉토리 위치는 OS 에서 ls 를 입력해보면 

![29](https://github.com/user-attachments/assets/6b12705e-969e-4dba-bdc2-6d7c9ddd95b5)

위 사진과 같은 결과가 나오게 됩니다.

다음으로 rm 을 해봅시다. 디렉토리 위치는 OS에서 rm Windows -r 을 입력해 주시면 

![30](https://github.com/user-attachments/assets/e9fc025d-2735-4a09-b534-6ceb518dab1a)

사진처럼 삭제 된것을 볼수 있습니다.

Windows 를 삭제시켰다면 mv를 이용해 봅시다.
cd 를 입력해 상위 디렉토리로 이동하고 난후 mkdir Windows 를 "home/username/" 위치의 하위 디렉토리로 만들어 줍시다.

![31](https://github.com/user-attachments/assets/3ca5e4d3-0ffc-4810-940a-7208f0d3c4a3)

이제 여기서 mv Windows /home/(사용자명)/을 입력하여서 위치를 옮겨줍시다.

![32](https://github.com/user-attachments/assets/5645c746-72d3-48c6-80a2-f5dfc38d5090)

이번시간은 여기까지 알아보도록 합시다.
