# book_linuxkernel_md

https://gurugio.gitbooks.io/book_linuxkernel_md/content/

커널의 간단한 블럭 장치 드라이버와 블럭레이어에 대한 분석을 해봤으니 이번에는 실제로 사용되는 블럭 장치 중에서 md 드라이버를 분석해보겠습니다.

md(software raid)드라이버를 이해하기 위해서는 디바이스 드라이버 자체와 md 장치를 생성하고 관리하는 mdadm 툴을 알아야합니다.
우선 mdadm툴로 md 장치가 어떻게 생겨나는지, 툴에서 어떤 명령들을 커널 드라이버에 전달하는지 등을 분석해보고,
그 다음에 커널 드라이버의 코드를 읽어보겠습니다.





