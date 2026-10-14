# ESOFT2-LTP-AULA10-TRABALHO-1

**Aluno(a):** [Digite seu nome]  
**Disciplina:** Linguagem e Técnicas de Programação  
**Professor:** José Carlos Flores

## Exercícios de PHP

### 1. Qual será a saída?

**Resposta esperada pelo material: `15`.** O material considera que a string `"10abc"` é convertida para `10` na soma com `5`, resultando em `15`. O comportamento pode variar conforme a versão do PHP.

### 2. Converta a string `"3.1415"` para inteiro e depois para booleano.

**Resultado:** `Inteiro: 3, Booleano: true`.

A conversão para inteiro descarta a parte decimal, ficando `3`. Como `3` não é zero, sua conversão para booleano é `true`.

### 3. Função para mostrar o tipo e o valor convertido para string

```php
function mostrarTipoEString($valor) {
    $tipo = gettype($valor);
    $comoString = (string)$valor;

    return "Tipo: $tipo, Valor como string: '$comoString'";
}

echo mostrarTipoEString(true);
```

`gettype()` identifica o tipo original da variável e `(string)` converte o valor para texto. Neste exemplo, `true` é convertido para `"1"`.

### 4. Corrija o código para evitar erro

```php
$idade = "vinte e cinco";

if (is_numeric($idade)) {
    $total = (int)$idade + 10;
    echo $total;
} else {
    echo "Idade inválida.";
}
```

`is_numeric()` verifica se o valor é numérico antes de fazer a conversão e a soma. Como `"vinte e cinco"` está por extenso, o programa mostra `Idade inválida.`. Para aceitar números escritos por extenso, seria necessário convertê-los para valores numéricos primeiro.

## Questionário sobre sessões em PHP

1. **B) Iniciar ou retomar uma sessão.** `session_start()` inicia uma sessão ou retoma uma existente.
2. **C) No servidor web.** Os dados de `$_SESSION` ficam armazenados no servidor.
3. **D) `valida.php`.** Esse arquivo valida os dados do login.
4. **D) `POST`.** Esse método envia os dados do formulário no corpo da requisição.
5. **B) Redirecionar o usuário.** `header('Location: painel.php')` direciona o navegador para outra página.
6. **B) Ocorre um erro de cabeçalho (“headers already sent”).** `session_start()` deve ser chamado antes de enviar conteúdo ao navegador.
7. **D) `$_SESSION`.** Essa superglobal armazena dados associados à sessão.
8. **B) Verificar `$_SESSION['logado']`.** A verificação pode impedir o acesso ao painel sem login.
9. **A) `css/estilo.css`.** Esse é o caminho indicado entre as alternativas para o arquivo CSS.
10. **A) Apagar os dados da sessão.** `session_destroy()` encerra a sessão atual.
11. **B) Prevenir ataques XSS.** `htmlspecialchars()` trata caracteres especiais para que não sejam interpretados como código HTML ou JavaScript.
12. **C) `<link>`.** Essa tag vincula um arquivo CSS externo ao HTML.
13. **B) Método não permitido.** HTTP 405 indica que o método usado não é aceito para aquele recurso.
14. **B) `C:\xampp\htdocs\`.** Essa é a pasta padrão do XAMPP para arquivos servidos pelo Apache.
15. **B) Evitar a execução do código posterior.** `exit;` encerra o script após o redirecionamento.
16. **C) Operador de coalescência nula.** `$_POST['usuario'] ?? ''` usa uma string vazia se o valor não existir ou for nulo.
17. **C) `true`.** Esse é o valor de `$_SESSION['logado']` após login bem-sucedido.
18. **C) `login.html`.** É o arquivo HTML entre as alternativas.
19. **B) A sessão é destruída e o usuário sai.** Essa é a função de `logout.php` no sistema descrito.
20. **D) Porta 80.** Essa é a porta padrão do Apache no XAMPP, salvo alteração na configuração.

## Identificação para envio

**Assunto do e-mail:** `ESOFT2-LTP-AULA10-TRABALHO-1`  
**Professor:** [jose.flores@unicesumar.edu.br](mailto:jose.flores@unicesumar.edu.br)

