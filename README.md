# Atividade_HTML
<!DOCTYPE html>
<html>
<head>
  <title>Calculadora de Área de Retângulo</title>
</head>
<body>
  <h1>Calculadora de Área de Retângulo</h1>
  <label for="base">Digite a base do retângulo:</label>
  <input type="number" id="base" />
  <br />
  <label for="altura">Digite a altura do retângulo:</label>
  <input type="number" id="altura" />
  <br />
  <button onclick="calcularArea()">Calcular Área</button>
  <br />
  <p id="resultado"></p>

  <script>
    function calcularArea() {
      // Obtém os valores digitados pelo usuário
      var base = parseFloat(document.getElementById('base').value);
      var altura = parseFloat(document.getElementById('altura').value);

      // Calcula a área do retângulo
      var area = base * altura;

      // Exibe o resultado da área
      var resultadoElement = document.getElementById('resultado');
      resultadoElement.innerHTML = 'A área do retângulo é: ' + area;
    }
  </script>
</body>
</html>
