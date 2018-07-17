# VueJS-Nginx


## Docker command


### without override default.conf

`docker run --name tmp-nginx-container -v $(pwd)/dist:/usr/share/nginx/html:ro --rm  -p 80:80  nginx`

### override default.conf
`docker run - name tmp-nginx-container -v $(pwd)/dist:/usr/share/nginx/html:ro -v $(pwd)/default.conf:/etc/nginx/conf.d/default.conf:ro - rm -p 80:80 nginx`
