# 1. Base 이미지 지정
FROM nginx
# 2. 외부(Jenkins)에서 전달받을 수 있는 ARG 선언(기본값 production 지정)
ARG NODE_ENV=production
# 3.  전달받은 ARG 값을 컨테이너 내부의 ENV(환경 변수)로 할당
ENV NODE_ENV=${NODE_ENV}
# 4.기본 작업 디렉터리 설정
WORKDIR /usr/share/nginx/html
# 5. 간단한 안내용 index.html 생성 (선택 사항)
RUN echo "<h1>Nginx Container $NODE_ENV</h1>" > index.html
EXPOSE 80