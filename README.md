# RA3_2
# Analisador LL(1) e Semântico
## Objetivo
Implementação das Fases 1, 2 e 3: gramática LL(1), parser e análise semântica que anota a AST com tipos. A entrada lógica da Fase 3 é a AST da Fase 2, a gramática de atributos e a tabela de símbolos; a saída é a AST anotada ou erro semântico.

## Como compilar
```bash
.\compile_fase3.bat
```
ou diretamente por comando caso o arquivo de compilação esteja faltante.
```bash
g++ -std=c++17 -O2 -Wall \
  main.cpp gramatica.cpp parser.cpp arvore.cpp leitor.cpp \
  tabela_simbolos.cpp semantico_driver.cpp semantico_inferencia.cpp \
  semantico_saida.cpp semantico_comandos.cpp \
  -o AnalisadorCompleto
```
## Como executar
```bash
.\AnalisadorCompleto.exe teste1.txt
```
## Entrada
Um artigo contendo o código-fonte da linguagem utilizada neste projeto (uma expressão RPN por linha) em formato .txt contendo apenas caracteres ASCII.

Exemplo:
```scss
teste
```
