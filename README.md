# Documentação do Formulário de E-mail

## Introdução
Este projeto consiste em um formulário interativo para a coleta de endereços de e-mail, utilizando HTML, Bootstrap e JavaScript para validação no lado do cliente. A validação assegura que os e-mails inseridos sigam um formato correto antes de serem processados.

## Tecnologias Utilizadas
- **HTML5**: Estruturação da página.
- **Bootstrap 5.3**: Estilização e componentes interativos.
- **JavaScript**: Validação do campo de e-mail e exibição de mensagens em um modal.

## Estrutura do Projeto
O projeto é composto pelos seguintes elementos:

### 1. Formulário de E-mail
O formulário contém:
- Um campo de entrada de texto para o e-mail.
- Um botão de envio.

### 2. Validação
A validação é feita em JavaScript utilizando a expressão regular:
```
/^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/
```
Esta expressão verifica se o e-mail segue o formato correto, como "exemplo@dominio.com".

### 3. Exibição de Mensagens
As mensagens de erro ou sucesso são exibidas em um modal Bootstrap. As verificações incluem:
- Campo vazio: "O campo de e-mail não pode estar vazio."
- Formato inválido: "Por favor, insira um e-mail válido."
- Formato correto: "E-mail válido! Formulário enviado com sucesso."

## Funcionamento
1. O usuário insere um e-mail no campo de entrada.
2. Ao pressionar o botão "Enviar", o JavaScript valida o campo:
   - Se estiver vazio ou inválido, uma mensagem de erro será mostrada no modal.
   - Se for válido, uma mensagem de sucesso será exibida.

## Dependências
O projeto utiliza o Bootstrap via CDN:
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

## Conclusão
Este projeto demonstra boas práticas para validação de formulários na web, garantindo uma melhor experiência do usuário e reduzindo erros de entrada de dados.

