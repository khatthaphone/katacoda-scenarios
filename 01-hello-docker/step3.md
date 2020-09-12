## ການເຂົ້າເຖິງ Container

ທຳອິດໃຫ້ຣັນ Nginx
`docker run -p 80:80 --name nginx nginx`

ເຂົ້າເຖິງ  Container ດ້ວຍຄຳສັ່ງ exec
`docker exec -it nginx bash`

ແກ້ໄຂໜ້າເວັບ
`vim /var/www/html/index.html`