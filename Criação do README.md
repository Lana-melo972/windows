#     __*Batch*__
 

### O que é?

O Batch Scripting funciona através da interpretação dos comandos contidos no arquivo .bat pelo interpretador de comandos do Windows. Quando o arquivo .bat é executado, o interpretador de comandos lê linha por linha do arquivo e executa os comandos correspondentes.

## *Como funcionam os comandos Batch?*

1. __*Execução de comandos no CMD*__: O arquivo Batch é composto por uma sequência de comandos do CMD que são executados na ordem em que aparecem no arquivo. Quando você executa um arquivo .bat, o sistema operacional Windows executa os comandos um por um.

2. __*Comandos comuns*__: Alguns dos comandos mais utilizados em scripts Batch são:

- ```echo```: Exibe uma mensagem na tela.


```   
batch

echo Hello, World!
```


- ```dir```: Lista arquivos e pastas do diretório atual.

```
batch

dir
```
- ```cd```: Muda o diretório atual.

```
batch

cd C:\Users
```


- ```pause```: Pausa a execução do script até que o usuário pressione uma tecla.

```
batch

pause
```

3. __*Estruturas de controle*__: Você também pode usar estruturas condicionais e loops para controlar o fluxo do script:


- ```if``` - Condicional:
```
batch

if exist arquivo.txt echo O arquivo existe.
```

- ```for``` - Laços de repetição:
```
batch

for %%i in (*.txt) do echo %%i
```

4. __*Variáveis*__: As variáveis podem ser usadas para armazenar dados temporários. Elas podem ser definidas e utilizadas dentro do script:
```
batch

set var=Olá
echo %var%
```
5. __*Comentários*__: Para adicionar comentários no código (que não serão executados), você usa ```rem``` ou ```:::```


```
batch

rem Este é um comentário
:: Outro comentário
```

6. __*Redirecionamento de saída*__: É possível redirecionar a saída de comandos para arquivos ou outros destinos. Por exemplo:

```
batch

dir > lista.txt
```

7. __*Encerramento do script*__: Você pode encerrar a execução do script com o comando exit:

```
batch

exit
```

__*Exemplo simples de script Batch*__

Aqui está um exemplo de um script simples que cria um diretório e copia um arquivo:

```
batch

@echo off
rem Cria um diretório chamado "meus_arquivos"
mkdir C:\meus_arquivos

rem Copia o arquivo "documento.txt" para o novo diretório
copy C:\documento.txt C:\meus_arquivos\

rem Pausa para visualizar a mensagem
pause
```

__*Como rodar um arquivo Batch:*__

1. Abra o Bloco de Notas ou qualquer editor de texto.

2. Escreva os comandos Batch que você deseja.

3. Salve o arquivo com a extensão .bat, por exemplo, meu_script.bat.

4. Para rodar, basta clicar duas vezes no arquivo ou executá-lo a partir do Prompt de Comando.

*Os scripts Batch são bastante úteis para tarefas de automação simples no Windows, como copiar arquivos, criar backups, ou até gerenciar configurações do sistema.*



...

[Message clipped]  View entire message
