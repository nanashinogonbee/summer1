Из этого репозитория создаётся контейнер с помощью автобилда за счёт связи с Docker Hub

При пушах контейнер автоматически перестраивается





```bash


docker run -itd -p 4321:4321 igossoudarev/summer1

curl "localhost:4321/summer?n1=2&n2=5&cors" -H 'Accept:application/json' -i

curl "localhost:4321/summer?n1=2&n2=5&cors" -H 'Accept:text/html'

curl "localhost:4321/summer/2/9" -H 'Accept:text/html' -i

curl "localhost:4321/summer/2/9?cors" -H 'Accept:text/html' -i

---

curl "kodaktor.ru/api/summer?n1=2&n2=5&cors" -H 'Accept:text/html' -iL

curl "kodaktor.ru/api/summer?n1=2&n2=5&cors" -H 'Accept:application/json' -iL

curl "kodaktor.ru/api/summer/4/11?cors" -H 'Content-Type:application/json' -iL

curl "kodaktor.ru/api/summer/4/11?cors" -H 'Content-Type:text/html' -iL


```
