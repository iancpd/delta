<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Área Protegida</title>
</head>
<body style="text-align:center; font-family:sans-serif; margin-top:100px;">
  <h2>Digite a senha para acessar:</h2>
  <input type="password" id="senha" placeholder="Senha">
  <button onclick="verificarSenha()">Acessar</button>
  <p id="erro" style="color:red;"></p>

  <script>
    function verificarSenha() {
      const senhaCorreta = "1234"; // 🔑 Troque pela sua senha
      const destino = "https://seulink.com"; // 🌐 Troque pela URL real
      const senhaDigitada = document.getElementById("senha").value;

      if (senhaDigitada === senhaCorreta) {
        window.location.href = destino;
      } else {
        document.getElementById("erro").innerText = "Senha incorreta!";
      }
    }
  </script>
</body>
</html>
