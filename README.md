# labredes21host
# labredes21
## Projeto final labredes2021 server tcp e apache

## Docker básico
construir uma aplicação com 3 serviços: Monitor, servidor tcp e servidor apache.

Monitor: [Presente em outro repositório](https://github.com/hitalofm/labredes21). Gera testes de ping, DNS e Getrequest.
server: Salva os testes em um arquivo html.
Apache: cria um http server e mostrar os testes.

## Executando o container server tcp e apache:

- sudo docker run --rm -p 8081:8081 -v "$(pwd):/app/www" --name=tcpserver labredes21/labredes21server python3 server.py 8081

- sudo docker run -it --rm --name my-apache-app -p 8080:80 -v "$PWD":/usr/local/apache2/htdocs/ httpd:2.4
