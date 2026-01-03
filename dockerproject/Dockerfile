# node 환경 고정
FROM node:20-alpine

WORKDIR /app

# 의존성 먼저 복사 → 빌드 캐시 활용
COPY package*.json ./
RUN npm install

# 전체 복사
COPY . .

# 빌드
RUN npm run build
