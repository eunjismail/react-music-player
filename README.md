22500029 고은지
# Project Information
### 프로젝트 소개
음악을 재생할 수 있는 플레이리스트입니다. 여러가지 음악을 마음대로 들을 수 있습니다.
### 선택 이유
저는 평상시에 걸으면서 음악 듣는 것을 좋아하기 때문에 저의 플레이리스트를 만들어 보고 싶었습니다. 프로젝트를 선택하기 전에, 코드도 보기 좋게 짜여 있다고 생각이 들어 해당 프로젝트로 선택하였습니다.
### 원본 GitHub URL 및 라이선스
https://github.com/M-R-Subash/react-music-player
This project is open source and available under the [MIT License](LICENSE).
## 👨‍💻 Developer
**Subash M R**  
- Portfolio: [https://bit.ly/4ls0iwK]
- GitHub: [@M-R-Subash](https://github.com/M-R-Subash)
- Email: mrsubash1615@gmail.com

# Installation
1. **Clone the repository**
   git clone https://github.com/M-R-Subash/react-music-player.git dependenciesgit
   cd react-music-player
2. **Install dependencies**
   npm install
3. **Start the development server**
   npm run dev
- 사진 :
![사진](./photos/photo.png)


### Project Structure: 주요 파일 2~3개의 역할
index.html은 하나만 존재하며, div에 react화면이 들어가는 것이다. 그리고 main.html의 script를 보면 /src/main.jsx로 연결되어 있고, 해당 파일로 이동하면 ./App.jsx로 연결되어 있다.
App.jsx에서는 웹페이지의 메인 화면과 주요 기능들을 구성하고 있다. 많은 함수가 있는데, 조금 말해보면 다음 노래, 이전 노래로 이동할 수 있는 기능이 존재한다.
### React Component: 주요 컴포넌트 1~2개의 역할
Player가 있다. player의 음악과 관련된 것을 담당하는 컴포넌트이다. 지금 재생되는 노래와 소리 조절, 다음 노래 / 이전 노래로 이동하는 기능 등을 제공하고 있다.
### Code Analysis: 코드 1개(약 5~15줄)를 선택하여 동작 원리 설명
App.jsx의 다음 곡으로 바꿔주는 handleNext() 함수에 대해서 동작 원리를 설명하려고 합니다. 우선 findIndex를 통해서 현재 실행되고 있는 음악이 몇번째인지 찾습니다. 그리고 그걸 currentIndex에 저장하고, +1을 한 것을 nextindex에 저장해서 다음 곡 위치를 알아내는 것입니다. 그리고 여기서 songs.length를 통해서 마지막 곡이 되면, 다음에는 첫번째 곡으로 돌아가게 설정해주는 것입니다. 그리고 setCurrentSong으로 지금 음악을 다음 음악으로 최종 변경해주는 동작 원리입니다.

# 수정 기록 
### Text 수정
제목을 변경했다.
수정 파일 : src/App.jsx
변경 전 : React Music Player
변경 후 : O(op)SSssss.. music playlist
OSS를 조금 바꾸어 oops를 합치고 싶었다.
### Style 수정
배경색과 컴포넌트 색상을 변경하였다.
수정파일 : src/App.jsx, src/components/Player.jsx, src/components/SongList.jsx
변경 전 : bg-gray-900, bg-gray-800, bg-gray-800
변경 후 : bg-pink-500, bg-pink-200, bg-pink-200
나의 플레이리스트니, 내가 좋아하는 색상으로 변경하였다.
### UI/DATA 수정
음악 개수를 표시할 수 있게 변경하였다.
수정파일 : src/App.jsx
변경 전 : 아무것도없음
변경 후 : <p>Total Songs: {songs.length}</p> 추가
몇개의 음악이 있는지 보고 싶어서 추가했다.






