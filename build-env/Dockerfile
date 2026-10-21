# 1. Base 이미지 지정
FROM nginx
# 2. 파이프라인에서 전달받을 build-arg 선언
ARG NODE_ENV=production
# 3. 컨테이너 내부 작업 디렉터리 설정
WORKDIR /usr/share/nginx/html
# 4. 간단한 안내용 index.html 생성 (선택 사항)
RUN echo "<h1>Nginx Container</h1>" > index.html
EXPOSE 80