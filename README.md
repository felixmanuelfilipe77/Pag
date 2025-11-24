<!--
Projeto: Website estático (HTML único)
Instituição: Escola Ténica de Informática (fictícia, Angola)
Objetivos cobertos:
 - Estrutura básica HTML5
 - Tags semânticas (header, nav, main, section, article, footer, aside)
 - Texto, cabeçalhos, parágrafos, quebras, alinhamento e cores (uso didático de atributos/elementos)
 - Imagens (<img> com src, alt, width, align) e imagem de fundo
 - Listas (ul, ol, dl) e listas aninhadas
 - Tabelas (<table>, <tr>, <td>) incluindo organização de informação complexa
 - Formulários (<form>, <input>, textarea, select, button)
 - Links (internos âncoras, externos, mailto)
 - Apenas HTML (todas as regras e estilos foram escritos inline/atributos para fins pedagógicos)

Salve este ficheiro como: index.html e abra num navegador.
--><!DOCTYPE html><html lang="pt-AO">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Escola Técnica Nova Esperança — Página Principal</title>
  <!-- Pequeno bloco de estilo inline para melhorar legibilidade (ainda dentro de HTML) -->
  <style>
    /* Aplica uma fonte legível e espaçamento básico para demonstração (válido dentro de HTML) */
    body { font-family: Arial, Helvetica, sans-serif; line-height: 1.45; margin: 0; padding: 0; }
    header, nav, main, footer, section, article, aside { display: block; }
    nav a { margin-right: 12px; text-decoration: none; }
    .container { width: 94%; max-width: 1100px; margin: 0 auto; padding: 16px; }
    .hero { padding: 24px 16px; border-radius: 8px; }
    .cards { display: flex; gap: 12px; flex-wrap: wrap; }
    .card { flex: 1 1 280px; padding: 10px; border-radius: 6px; }
    table { border-collapse: collapse; width: 100%; }
    table td, table th { border: 1px solid #999; padding: 8px; }
    footer { font-size: 0.9rem; padding: 12px 0; text-align: center; }
    /* Nota pedagógica: usamos style dentro do HTML por simplicidade do exercício */
  </style>
</head>
<body style="background-color:#f6f7fb; color:#222;">
  <header style="background-image: url('https://via.placeholder.com/1400x300?text=Escola+T%C3%A9cnica+Nova+Esperan%C3%A7a'); background-size: cover; background-position: center;">
    <div class="container">
      <h1 style="color: white; text-shadow: 1px 1px 2px rgba(0,0,0,0.6);">Escola Técnica Nova Esperança</h1>
      <p style="color: white; margin-top: -6px;">Formação técnica para jovens angolanos — prática, ética e futuro.</p>
      <nav aria-label="Navegação principal" style="margin-top:12px;">
        <!-- links internos (âncoras) -->
        <a href="#sobre">Sobre</a>
        <a href="#cursos">Cursos</a>
        <a href="#horarios">Horários & Tabela</a>
        <a href="#inscricao">Inscrição</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </div>
  </header>  <main class="container">
    <section id="sobre" class="hero" style="background-color:#ffffff; margin-top:16px;">
      <article>
        <h2>Sobre a Escola</h2>
        <p>A <strong>Escola Técnica Nova Esperança</strong> é uma instituição fictícia criada para este exercício. Tem como missão proporcionar competências técnicas em áreas como Informática, Eletricidade e Gestão para jovens de Angola.</p>
        <p>Localização: <em>Luanda, Angola</em> — entre as comunidades e empresas locais para favorecer estágios práticos.</p>
        <!-- imagem com atributos apropriados -->
        <img src="https://via.placeholder.com/640x360?text=Aula+Pr%C3%A1tica" alt="Alunos em aula prática" width="640" align="right" style="margin-left:12px;">
        <p>Utilizamos metodologias ativas. Os cursos combinam teoria e prática, com oficinas e projetos reais.</p>
      </article>
    </section><section id="cursos" style="margin-top:18px;">
  <h2>Cursos Oferecidos</h2>
  <div class="cards">
    <div class="card" style="background-color:#fff;">
      <h3>Informática</h3>
      <ul>
        <li>Introdução à informática</li>
        <li>Programação (HTML, CSS, JS) — nível básico</li>
        <li>Manutenção de Hardware</li>
        <!-- lista aninhada para mostrar níveis -->
        <li>Projeto prático:
          <ol>
            <li>Montagem de PC</li>
            <li>Instalação de sistema</li>
            <li>Criação de página web simples</li>
          </ol>
        </li>
      </ul>
    </div>

    <div class="card" style="background-color:#fff;">
      <h3>Eletricidade</h3>
      <ul>
        <li>Fundamentos de eletricidade</li>
        <li>Instalações residenciais</li>
        <li>Segurança no trabalho</li>
      </ul>
    </div>

    <div class="card" style="background-color:#fff;">
      <h3>Gestão e Empreendedorismo</h3>
      <dl>
        <dt>Objetivo</dt>
        <dd>Preparar jovens para gerir pequenos negócios e projetos comunitários.</dd>
        <dt>Conteúdo</dt>
        <dd>Finanças básicas, marketing local e elaboração de planos.</dd>
      </dl>
    </div>
  </div>
</section>

<section id="horarios" style="margin-top:18px; background:#fff; padding:12px; border-radius:6px;">
  <h2>Horários & Grade</h2>
  <p>A tabela abaixo organiza os cursos por dia, horário e sala — ideal para visualizar informação complexa de forma tabular.</p>

  <!-- Tabela demonstrativa com organização complexa -->
  <table aria-describedby="descricaoTabela">
    <caption id="descricaoTabela">Grade semanal (amostra)</caption>
    <thead>
      <tr>
        <th>Dia</th>
        <th>08:00 - 10:00</th>
        <th>10:30 - 12:30</th>
        <th>14:00 - 16:00</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Segunda</td>
        <td>Informática — Sala A</td>
        <td>Eletricidade — Oficina 1</td>
        <td rowspan="2">Atividades Práticas / Projetos</td>
      </tr>
      <tr>
        <td>Terça</td>
        <td>Gestão — Sala B</td>
        <td>Informática — Laboratório</td>
      </tr>
      <tr>
        <td>Quarta</td>
        <td>Eletricidade — Oficina 1</td>
        <td>Gestão — Sala B</td>
        <td>Manutenção & Suporte</td>
      </tr>
      <tr>
        <td>Quinta</td>
        <td colspan="2">Laboratório aberto para estágios (08:00 - 12:30)</td>
        <td>Workshops convidados</td>
      </tr>
      <tr>
        <td>Sexta</td>
        <td>Revisões e Avaliações</td>
        <td>Projetos em grupo</td>
        <td>Encerramento semanal</td>
      </tr>
    </tbody>
  </table>

</section>

<section id="inscricao" style="margin-top:18px;">
  <h2>Inscrição</h2>
  <p>Preencha o formulário abaixo para manifestar interesse. (Exercício prático de formulários em HTML)</p>

  <form action="#" method="post" enctype="application/x-www-form-urlencoded">
    <fieldset>
      <legend>Dados Pessoais</legend>
      <label for="nome">Nome completo:</label><br>
      <input type="text" id="nome" name="nome" placeholder="Ex: João Silva" required><br><br>

      <label for="email">Email:</label><br>
      <input type="email" id="email" name="email" placeholder="exemplo@dominio.com" required><br><br>

      <label for="curso">Curso de interesse:</label><br>
      <select id="curso" name="curso">
        <option value="informatica">Informática</option>
        <option value="eletricidade">Eletricidade</option>
        <option value="gestao">Gestão</option>
      </select><br><br>

      <label>Preferência de horário:</label><br>
      <input type="radio" id="manha" name="turno" value="manha" checked>
      <label for="manha">Manhã</label>
      <input type="radio" id="tarde" name="turno" value="tarde">
      <label for="tarde">Tarde</label><br><br>

      <label for="bio">Breve apresentação (máx. 300 caracteres):</label><br>
      <textarea id="bio" name="bio" rows="4" cols="40" maxlength="300"></textarea><br><br>

      <label for="ficheiro">Anexar comprovativo (opcional):</label><br>
      <input type="file" id="ficheiro" name="ficheiro" accept=".pdf,.jpg,.png"><br><br>

      <button type="submit">Enviar inscrição</button>
    </fieldset>
  </form>

</section>

<aside style="margin-top:18px; background:#fff; padding:12px; border-radius:6px;">
  <h3>Recursos & Links</h3>
  <ul>
    <li>Material de apoio: <a href="https://example.com/manual" target="_blank" rel="noopener">Guia do aluno (exemplo)</a></li>
    <li>Email de contacto: <a href="mailto:secretaria@novaesperanca.ao">secretaria@novaesperanca.ao</a></li>
    <li>Mapa de como chegar (link externo): <a href="https://maps.example.com" target="_blank">Ver no mapa</a></li>
  </ul>
</aside>

<section id="contacto" style="margin-top:18px;">
  <h2>Contacto</h2>
  <p>Telefone: <strong>+244 222 000 000</strong></p>
  <p>Endereço: Rua Exemplo, Luanda</p>

  <h3>Formas rápidas</h3>
  <ol>
    <li>Enviar email através do link <a href="mailto:direcao@novaesperanca.ao">direcao@novaesperanca.ao</a>.</li>
    <li>Visitar a secretaria em horário laboral.</li>
    <li>Preencher o formulário de inscrição acima.</li>
  </ol>

  <!-- link interno para voltar ao topo -->
  <p><a href="#top">Voltar ao topo</a> <!-- âncora interna --> </p>
</section>

  </main>  <footer style="background:#222; color:#fff; margin-top:18px;">
    <div class="container">
      <p>&copy; 2025 Escola Técnica Nova Esperança — Material didático (fictício).</p>
      <p>Desenvolvido em HTML5 — exercício que demonstra uso de tags semânticas, imagens, tabelas, listas, formulários e links.</p>
    </div>
  </footer>
</body>
</html>