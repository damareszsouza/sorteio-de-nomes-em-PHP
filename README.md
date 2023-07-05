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

# 10 codigos úteis em PHP 

# 01. Buscar um caracter específico em uma string e substitui-lo por outro
   
$texto = 'oi-eu-sou-um-texto';
$resultado = str_replace('-', ' ', $texto);
echo $resultado; // oi eu sou um texto

# 2. Fazer uma comparação If/Else em uma linha

$var1 = 5;
$var2 = 1;
echo $var1 > $var2 ? 'var1 é maior que var2' : 'var2 é maior que var1'; // condição ? caso true : caso false

# 3. Obter a URL da página em que se está em PHP

$url = $_SERVER['HTTP_HOST'];
echo 'A URL atual é '.$url;

# 4. Redirecionamento de endereço em PHP

header('Location: https://www.eufacoprogramas.com'); // Redireciona o usuario para eufacoprogramas.com

# 5. Como detectar o navegador do usuário em PHP

$useragent = $_SERVER['HTTP_USER_AGENT'];
echo "<strong>Seu navegador é</strong>: " . $useragent;

# 06. Validação de e-mail em PHP

$email = $_POST['email'];
if(!preg_match("/^[a-zA-Z0-9_.-]+@[a-zA-Z0-9-]+.[a-zA-Z0-9-.]+$/",$email)) {
echo 'Email inválido.';
}

# 07. Enviar e-mail em PHP

$dest = "destinatario@gmail.com"; //Email de destino
$assunto = "Assunto"; //Assunto
$corpo= "Corpo da mensagem. É permitido o uso de HTML."; //Corpo do e-mail
//Cabecalho do email
$headers = "De: Gabriella fonseca.gabriella@gmail.comrn"; //Remetente
$headers .= "X-Mailer: PHP5n";
$headers .= 'MIME-Version: 1.0' . "n";
$headers .= 'Content-type: text/html; charset=iso-8859-1' . "rn"; //
mail($dest,$assunto,$corpo,$headers);

# 8. Loop Simples

for($j = 0 ;$j < 10 ;$j++){
echo 'Essa frase vai ser escrita 10 vezes
';
}

# 09. Obter o IP do usuário.

Importante: Essa função não funciona localmente.

$ip = $_SERVER['REMOTE_ADDR'];
echo $ip;

# 10. Contar quantos caracteres ou palavras há em uma string

// Para contar caracteres
$str = 'abcdef';
echo strlen($str); // 6

// Para contar palavras
$str2 = 'aqui são quatro palavras';
echo str_word_count($str2); // 4
