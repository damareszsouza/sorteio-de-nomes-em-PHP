# sorteio-de-nomes-em-PHP
Praticas e estudos da linguagem PHP

Aqui está um exemplo de código PHP que pode ser usado para sortear nomes aleatórios:

<?php
$nomes = array("João", "Maria", "Pedro", "Lucas", "Ana", "Julia");
$sorteado = array_rand($nomes);
echo $nomes[$sorteado];
?>

Este código cria um array com os nomes que você deseja sortear e usa a função array_rand() para selecionar um nome aleatório do array. Em seguida, ele exibe o nome sorteado na tela.

#  Aqui está um exemplo de código em PHP para sorteio de números aleatórios:

<?php
$min = 1;
$max = 100;
echo rand($min,$max);
?>

Você pode alterar os valores de $min e $max para definir o intervalo de números que deseja sortear.

#Aqui está um exemplo de código PHP que gera números decrescentes:

<?php
// Gera números decrescentes em PHP
for ($i = 10; $i >= 1; $i--) {
    echo $i . '<br>';
}
?>

# Aqui está um exemplo de código PHP que gera números crescentes:

<?php
// Gera números crescentes em PHP
for ($i = 1; $i <= 10; $i++) {
    echo $i . '<br>';
}
?>

# Para buscar um caracter específico em uma string e substitui-lo por outro em PHP, você pode usar a função str_replace(). Esta função procura o substrato dado e substitui-o com o valor fornecido. A sintaxe correta para utilizar esta função é a seguinte:

str_replace($caracter_a_ser_substituido, $novo_caracter, $string);


Por exemplo, se você quiser substituir o caractere “a” pelo caractere “b” na string “banana”, você pode usar o seguinte código:

$string = "banana";
$nova_string = str_replace("a", "b", $string);
echo $nova_string; // "bbnbnb"

# operador ternario 

Para fazer uma comparação If/Else em uma linha em PHP, você pode usar o operador ternário. O operador ternário é uma forma abreviada de escrever uma instrução If/Else em uma única linha.

A sintaxe do operador ternário é a seguinte:

```php
$variavel = (condição) ? valor_se_verdadeiro : valor_se_falso;
```

Por exemplo, se você quiser verificar se um número é maior ou menor que 10 e atribuir um valor à variável com base no resultado da comparação, você pode usar o seguinte código:

```php
$numero = 5;
$resultado = ($numero > 10) ? "maior que 10" : "menor que 10";
echo $resultado; // "menor que 10"
```
 operador ternário nos seguintes links:

- [Operador Ternário no PHP - DevMedia](https://www.devmedia.com.br/operador-ternario-no-php/37289)
- [PHP - Operador Ternário - W3Schools](https://www.w3schools.com/php/php_operators.asp)
