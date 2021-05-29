# Docker.Ferramentas

## Rede padrão

Se quiser manter uma network default, execute o comando abaixo:

``` bash
docker create network dev_network
```

E nos arquivos `docker-compose.yml`, ficará o trecho abaixo:

``` yml
#...

networks: 
  default:
    external: 
      name: dev_network

#...
```

Caso queira que a network seja criada automaticamente, basta remover o trecho acima e desconsiderar o comando de criação da _network_.
