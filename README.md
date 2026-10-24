# Contador de palavras

Projeto de estudo em Python que lê documentos, conta as palavras
e apresenta até 10 palavras mais frequentes.

## Funcionalidades

- Leitura de arquivos TXT, DOCX e PDF com texto extraível.
- Contagem total de palavras.
- Exibição das palavras mais frequentes e suas quantidades.
- Contagem sem diferenciar letras maiúsculas e minúsculas.
- Aviso quando o arquivo não existe ou o formato não é suportado.

## Ferramentas utilizadas

- Python.
- python-docx, para leitura de documentos Word.
- pypdf, para extração de texto de PDFs.

## Como executar no Windows

É necessário ter Python instalado.

Abra o terminal na pasta principal do projeto.

### 1. Prepare o ambiente

Caso ainda não tenha um ambiente chamado venv neste projeto:

```powershell
python -m venv venv
```

### 2. Instale as bibliotecas

```powershell
.\venv\Scripts\python.exe -m pip install -r requirements.txt
```

### 3. Execute o programa

```powershell
.\venv\Scripts\python.exe contador.py
```

Quando o programa solicitar o caminho do arquivo, digite:

```text
exemplo.txt
```

## Exemplo de uso

Conteúdo do arquivo exemplo.txt:

```text
Python Python Git GitHub Python
```

Resultado esperado:

```text
O arquivo possui 5 palavras.
As 10 palavras mais frequentes são: [('python', 3), ('git', 1), ('github', 1)]
```

Como o exemplo possui apenas três palavras diferentes,
o programa apresenta três resultados, mesmo que o limite seja dez.

## Limitações atuais

- Arquivos TXT precisam estar salvos em UTF-8.
- PDFs que contêm apenas imagens não têm seu texto reconhecido.
- A contagem é simples e também pode incluir números.
- Alguns erros de leitura ainda precisam de mensagens mais claras.

## Próximas melhorias

- Melhorar a apresentação dos resultados.
- Criar testes automatizados.
- Tratar outros erros de leitura.

## Objetivo do projeto

Praticar Python, leitura de arquivos, contagem de ocorrências
e controle de versões com Git e GitHub.