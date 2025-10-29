<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulário de Dados Pessoais</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      padding: 20px;
    }
    form {
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      max-width: 400px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin-top: 10px;
      font-weight: bold;
    }
    input, select, textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      margin-top: 15px;
      background-color: #4CAF50;
      color: white;
      padding: 10px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <h2>Formulário de Dados Pessoais</h2>

  <form action="#" method="post">
    <label for="nome">Nome Completo:</label>
    <input type="text" id="nome" name="nome" required>

    <label for="data">Data de Nascimento:</label>
    <input type="date" id="data" name="data" required>

    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email" required>

    <label for="telefone">Telefone:</label>
    <input type="tel" id="telefone" name="telefone" placeholder="+244 9xx xxx xxx" required>

    <label for="endereco">Endereço:</label>
    <textarea id="endereco" name="endereco" rows="3" placeholder="Rua, Bairro, Cidade"></textarea>

    <label for="genero">Gênero:</label>
    <select id="genero" name="genero">
      <option value="">Selecione</option>
      <option value="masculino">Masculino</option>
      <option value="feminino">Feminino</option>
      <option value="outro">Outro</option>
    </select>

    <button type="submit">Enviar</button>
  </form>

</body>
</html>