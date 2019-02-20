https://davemateer.com/2018/01/25/Jekyll-and-Docker

https://linuxize.com/post/how-to-remove-docker-images-containers-volumes-and-networks/

cd c:/temp/myBlog

run Jekyll
docker run --rm -v=%cd%:/srv/jekyll -it jekyll/jekyll /bin/bash

serving site locally
docker run --rm -v=%cd%:/srv/jekyll -p 4000:4000 -it jekyll/jekyll /bin/bash

serving jekyll on port 4000
jekyll serve --force_polling