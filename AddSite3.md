# How to add Site3 in your project
1. 
2. Copy this fragment into docker-compose.yml 
```
nginx-site3:
    image: nginx:latest
    container_name: site3
    labels:
      - "traefik.enable=true"
      - "traefik.http.routers.site3.rule=Host(`site3.user.parseq.pro`)"
      - "traefik.http.routers.site3.entrypoints=websec"
      - "traefik.http.routers.site3.tls=true"
      - "traefik.http.routers.site3.tls.certresolver=le"   
    volumes:
      - ./site3/:/usr/share/nginx/html
```
3. Create site3 directory in your poject directory
4. Create or put index.html file in your site3 directory
5. `docker-compose down && docker-compose up -d`
