# Laboratório web para balanceadores F5-LTM

Este ambiente é composto de dois containers nginx (Alpine) com uma página web simples com múltiplas imagens. A intenção é facilitar os laboratórios de estudos dos balanceadores de carga F5, com foco no módulo LTM.

## Instalação

Utilize o docker-compose para subir os containers para facilitar.

```bash
docker-compose up 
```

## Utilização

Em cada container nginx existem 3 "sites" hospedados. Um que atende o "/", o site1, que atende no "/site1" e por fim o site2 disponível em "/site2". Apesar de parecidos, o conteúdo das imagens são um pouco diferentes. Com isso, é possível ver o path utilizado para carregar as imagens.

Servidor Green/Verde - Site Default - http://localhost:3000
Servidor Green/Verde - Site Site 1 - http://localhost:3000/site1
Servidor Green/Verde - Site Site 2 - http://localhost:3000/site2

Servidor Red/Vermelho - Site Default - http://localhost:3001
Servidor Red/Vermelho - Site 1 - http://localhost:3001/site1
Servidor Red/Vermelho - Site 2 - http://localhost:3001/site2


## License

[MIT](https://choosealicense.com/licenses/mit/)