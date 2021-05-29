# Portainer

Sobre os comandos, algumas observações:

## Volumes

- Em volumes, altere o trecho `- ./Portainer:/data` para o caminho desejado no seu ambiente. Desta forma, os dados do portainer serão mapeados localmente ao invés de ficar na imagem do Docker.
- Caso não queira utilizar desta forma, pode-se mapear o volume no próximo Docker, conforme a documentação oficial do Portainer: `portainer_data:/data`.
  - [Portainer CE](https://documentation.portainer.io/v2.0/deploy/ceinstalldocker/)

## Reinicialização

No trecho `restart: always`, indica que será reiniciado sempre que o container for interrompido. Ver [Start containers automatically](https://docs.docker.com/config/containers/start-containers-automatically/).
