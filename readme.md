# HTTP Server Go

Este projeto é o meu primeiro servidor web simples escrito em Go, que permite visualizar, editar e salvar páginas de texto, foi criado com base na documentação padrão do Go, visando aprender o básico para criação de aplicações web. Cada página é armazenada como um arquivo `.txt` no servidor, e pode ser acessada, modificada e salva através de uma interface web.

## Funcionalidades

- Visualizar páginas existentes (`/view/PAGENAME`)
- Editar páginas (`/edit/PAGENAME`)
- Salvar páginas editadas (`/save/PAGENAME`)
- Ao acessar uma página não existente com (`/edit/NEWPAGENAME`) será possível a criação de uma página nova
- Renderização de templates HTML para visualização e edição

## Como executar

1. Certifique-se de ter o Go instalado.
2. Coloque os arquivos `main.go`, `edit.html` e `view.html` no mesmo diretório.
3. Execute o servidor:

	```
	go run main.go
	```

4. Acesse `http://localhost:8080/view/PAGENAME` no navegador para criar ou visualizar páginas.

## Estrutura dos arquivos

- `main.go`: Código principal do servidor.
- `edit.html`: Template HTML para edição de páginas.
- `view.html`: Template HTML para visualização de páginas.

## Observações

- Os arquivos de página são salvos no formato `PAGENAME.txt` no diretório do servidor.
- O projeto é apenas para fins educacionais e não deve ser usado em produção sem melhorias de segurança.