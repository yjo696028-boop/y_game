# NEON//DUEL — 1대1 온라인 FPS

## 실행과 배포

`index.html`은 정적 웹페이지입니다. 두 사람이 각자 브라우저에서 접속하려면 이 파일을 HTTPS로 호스팅해야 합니다. 예를 들어 GitHub Pages, Netlify, Cloudflare Pages 같은 정적 사이트 호스팅에 `index.html`을 올리면 됩니다.

사이트에 접속한 뒤 한 명이 **방 만들고 초대 링크 복사**를 누르고, 복사된 링크를 친구에게 보내세요. 상대가 링크를 열면 방에 참가하고 전투가 시작됩니다. 호스트 페이지를 닫으면 방이 종료됩니다.

## 조작

- `W A S D`: 이동
- 마우스: 시야 회전
- 마우스 왼쪽 클릭: 발사 (화면을 클릭하면 마우스 조준이 고정됩니다)
- `R`: 재장전
- 상대에게 4발 명중하면 라운드 승리

## 연결 방식

실시간 게임 데이터는 WebRTC 피어 간에 전송하고, PeerJS Cloud는 초기 연결 신호 교환에 사용합니다. PeerJS 공식 안내에 따르면 기본 클라우드 서버는 별도 설정 없이 이용할 수 있으며, 고트래픽 서비스에는 자체 PeerServer를 권장합니다. 인터넷 환경이나 방화벽 설정에 따라 연결이 실패할 수 있습니다.

참고: [PeerJS 시작하기](https://peerjs.com/client/getting-started), [PeerJS Cloud](https://peerjs.com/server/cloud)
