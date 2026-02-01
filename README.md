
- Vale conferir a versao instalada antes de seguir os passos abaixo.

O desafio pede uma tela de acesso simples e, depois de autenticado, o envio de um arquivo qualquer.

O projeto foi feito em Rails, seguindo a estrutura padrão do framework.

---------------------

Enunciado original:

# Teste técnico - vaga de back-end

Leia este documento até o fim, com calma e atenção.
O objetivo aqui é medir o seu conhecimento técnico na parte de servidor, mais especificamente em Ruby.

A tarefa consiste em ler [um arquivo de texto no formato CNAB](https://github.com/Pagnet/desafio-back-end/blob/master/CNAB.txt) e gravar as informações de movimentação financeira num banco relacional, à sua escolha.

O trabalho é feito em casa, no seu ritmo. Normalmente não é preciso mais do que algumas horas.

# Como entregar

1. Primeiro, duplique o projeto para a sua conta no GitHub (crie uma, se ainda não tiver).
2. Em seguida, implemente conforme descrito abaixo, na sua cópia local.
3. Por último, envie por e-mail um arquivo de diferenças para o seu contato na empresa.

# Descrição

Você recebeu um arquivo com os lançamentos financeiros de várias lojas e precisa de um jeito de trazê-los para um banco de dados.

O trabalho é criar uma interface web que aceite o envio do arquivo, normalize o conteúdo, grave tudo num banco relacional e mostre o resultado na tela.

**A aplicação PRECISA:**

1. Ter uma tela com formulário para envio do arquivo
2. Interpretar o arquivo recebido, normalizar os campos e gravar corretamente, respeitando a documentação de layout abaixo
3. Listar as operações por loja, com o saldo totalizador por loja e o geral
4. Ser escrita em Ruby 2.0 ou superior
5. Ser simples de configurar e rodar em ambiente Unix (Linux ou macOS), usando apenas bibliotecas livres ou gratuitas

**A aplicação NÃO precisa:**

1. Tratar autenticação ou autorização — mas isso conta pontos extras, e mais ainda se for via OAuth
2. Usar um framework específico — se preferir usar um, sem problema, escolha o que fizer sentido

# Layout do arquivo

| Campo | Início | Fim | Tamanho | Comentário
| ------------- | ------------- | -----| ---- | ------
| Tipo  | 1  | 1 | 1 | Código da operação
| Data  | 2  | 9 | 8 | Data da ocorrência