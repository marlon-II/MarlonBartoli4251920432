# Verificador de palíndromos

## Objetivo do código

Esse código tem como objetivo verificar se duas frases são palíndromos ou não, ele realiza a verificação em frases pré-definidas no código.

## Como executar o código?

Esse é um código em Python, então para utiliza-lo você pode utilizar o Pycharm, Visual Studio Code ou mesmo o Codespace do GitHub.

**Passo a passo para utiliza-lo pelo Codespace:**

1. Realize o Fork do repositório;
1. Acesse o menu do GitHub;
2. Clique em Codespace;
3. Vai em "New Codespace";
4. Selecione o repositório e clique em "Create Codespace";
5. No menu da direita vai em extensões e procure a extensão de Python e baixe ele;
6. Aperte o botão rum (símbolo de player).

## Resultado de saída

A saída são duas Strings, afirmando que a primeira frase é falsa e a segunda é verdadeira, conforme exemplo abaixo:

```
Teste 1: False

Teste 2: True
```

Esse resultado se dar, pois o **Teste 1** utilizou a frase "A sacada da casa de cadasa", que não é um palíndromo e a frase do **Teste 2** é a "Socorram-me, subi no ônibus em Marrocos" e ela é um palíndromo.

## Papel do método "main"

Ele serve para rodar o script apenas quando utilizar o código diretamente sem utilizar uma automação, nesse método temos as frases que servirão para teste do código.

## Detalhamento do método "Analisar"

Esse método pegue a frase de entrada e deixa ela em minúsculo, sem caracteres especial e inverte ela, segue com o resumo de cada etapa:

#### Linha 4:

```
if entrada is None:
        return False
```

Aqui verifica se a entrada é vazia e caso seja o método retorna **False**.

#### Linha 8:

```
limpa = re.sub(r'[^a-zA-Z0-9]', '', entrada).lower()
```

Nessa linha, colocamos na variável "limpa" a string modificada sem os caracteres especiais, espaços e deixa em minúsculo.

#### Linha 11:

```
 invertida = limpa[::-1]
```

Aqui a variável "invertida" recebe a string presente em "limpa" de traz para frente.

#### Linha 13:

```
return limpa == invertida
```

Aqui verifica se a string presente em "limpa" é igual a string presente em "invertida".


## Motivo da saída

O resultado do código é

```
Teste 1: False

Teste 2: True
```

Esse resultado se dar, pois o **Teste 1** utilizou a frase "A sacada da casa de cadasa", que não é um palíndromo e a frase do **Teste 2** é a "Socorram-me, subi no ônibus em Marrocos" e ela é um palíndromo.

## Sobre

Esse Fork e documentação foi realizado pelo aluno **Marlon Andrade Bartoli** que tem o RA **4251920432**.
