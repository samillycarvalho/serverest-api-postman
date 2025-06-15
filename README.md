
  <h1>🧪 API Serverest - Testes Automatizados com Postman</h1>

  <p>
    Este repositório contém uma <strong>coleção de testes automatizados</strong> da API 
    <a href="https://serverest.dev/" target="_blank">Serverest</a> utilizando o <strong>Postman</strong>, 
    com foco em simular e validar os principais fluxos de uma aplicação RESTful — incluindo autenticação, 
    CRUD de usuários, produtos, carrinho, etc.
  </p>

  <h2>📁 Estrutura do Projeto</h2>
  <pre><code>
📦 serverest-api-postman/
├── README.md
├── collections/
│   └── Login.json
│   └── User.json
│   └── Product.json   
├── environments/
│   └── environment.json
├── globals/
│   └── globals.json    
  </code></pre>

  <h2>🚀 Como Executar os Testes</h2>
  <ol>
    <li>
      <strong>Clone o repositório:</strong>
      <pre><code>git clone https://github.com/samillycarvalho/api-serverest-postman.git</code></pre>
    </li>
    <li>
      <strong>Importe a Collection e o Environment no Postman:</strong>
      <ul>
        <li>Vá em <em>File > Import</em></li>
        <li>Selecione os arquivos <code>.json</code> da pasta <code>collections/</code> e <code>environments/</code></li>
      </ul>
    </li>
    <li>
      <strong>Configure as variáveis de ambiente:</strong>
      <ul>
        <li><code>{{url}}</code> → <code>https://serverest.dev</code></li>
        <li>Outras variáveis como <code>{{Auth}}</code> são preenchidas dinamicamente</li>
      </ul>
    </li>
    <li>
      <strong>Execute os testes:</strong>
      <ul>
        <li>No Postman, selecione a collection → clique em <strong>Run Collection</strong></li>
        <li>Escolha o environment <code>serverest-environment</code> e clique em <strong>Run</strong></li>
      </ul>
    </li>
  </ol>

  <h2>🧰 Tecnologias Utilizadas</h2>
  <ul>
    <li><strong>Postman</strong> para criação e execução dos testes</li>
    <li><strong>JavaScript</strong> nos scripts de teste</li>
    <li><strong>Variáveis de ambiente</strong> no Postman</li>
    <li><strong>Newman</strong> (opcional) para execução via terminal/CI</li>
  </ul>

  <h2>📊 Integração com Newman (opcional)</h2>
  <p>Para rodar os testes via terminal:</p>
  <ol>
    <li>Instale o Newman:
      <pre><code>npm install -g newman</code></pre>
    </li>
    <li>Execute:
      <pre><code>newman run user.postman_collection.json \
-e environments/serverest-environment.postman_environment.json</code></pre>
    </li>
  </ol>

  <h2>💡 Boas Práticas Aplicadas</h2>
  <ul>
    <li>Uso de <strong>variáveis dinâmicas</strong> e <strong>token automático</strong></li>
    <li>Organização dos requests por <strong>módulo</strong> (auth, usuários, produtos, etc.)</li>
    <li>Scripts de teste claros com validações de status, schema e mensagens</li>
    <li>Reutilização de dados e automação de fluxos</li>
  </ul>

  <h2>✅ Cobertura de Testes</h2>
  <table>
    <tr>
      <th>Módulo</th>
      <th>Status</th>
    </tr>
    <tr>
      <td>Auth</td>
      <td>✅ Testado</td>
    </tr>
    <tr>
      <td>Usuários</td>
      <td>✅ Testado</td>
    </tr>
    <tr>
      <td>Produtos</td>
      <td>✅ Testado</td>
    </tr>
    <tr>
      <td>Carrinho</td>
      <td>✅ Testado</td>
    </tr>
    <tr>
 
  </table>

</body>
</html>

