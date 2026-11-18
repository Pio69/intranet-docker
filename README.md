# Intranet

Site de intranet com páginas para acesso a informações e serviços, desenvolvido com HTML, CSS e JavaScript sobre o template AdminLTE. Este repositório reúne os arquivos do site e a configuração Docker.

## Estrutura

```text
app/              # páginas, imagens, estilos, scripts e recursos do AdminLTE
docker/Dockerfile # imagem Apache para servir o site
```

## Executar com Docker

Com o Docker instalado e em execução, na raiz do repositório:

```bash
docker build -f docker/Dockerfile -t intranet .
docker run --rm -p 8080:80 intranet
```

Acesse [http://localhost:8080](http://localhost:8080). Para encerrar, pressione `Ctrl+C` no terminal.

A imagem copia os arquivos locais de `app/` para o Apache. A aplicação contém páginas e recursos estáticos; o Dockerfile não configura serviços externos ou um backend de autenticação.

## Tecnologias

- HTML, CSS e JavaScript
- AdminLTE e bibliotecas incluídas no projeto
- Apache HTTP Server e Docker

 Os links e recursos externos presentes nas páginas podem depender de serviços de terceiros.
