FROM node

WORKDIR /app

# WORKDIR을 설정했기 때문에 .을 사용해도 된다.
# COPY package.json /app
COPY package.json .

RUN npm install

# 첫번째 . : 현재 디렉토리의 전체 폴더
# 두번째 . : 작업디렉토리
# COPY . /app
COPY . .

EXPOSE 80

# VOLUME ["/app/node_modules"]

VOLUME [ "/app/feedback" ]

CMD ["npm", "start"]