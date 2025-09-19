# Node.js 공식 경량 이미지 사용
FROM node:18

# 앱 디렉토리 생성
WORKDIR /usr/src/app

# package.json이 있다면 먼저 복사 후 npm install (여기서는 server.js만 있다고 하셨으니 npm install 필요없을 수도 있음)
# COPY package*.json ./
RUN npm init -y
RUN npm install

# 앱 소스 복사
COPY . .

# 80 포트로 서버 실행한다고 가정
EXPOSE 80

# 기본 실행 명령
CMD ["node", "server.js"]
