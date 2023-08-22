README - Execução do Script HTML, CSS, JS e Banco SQL
Este é um guia passo a passo para executar um projeto web de gerenciamento de campeonatos, que utiliza tecnologias HTML, CSS, JavaScript e um banco de dados SQL.

Descrição da Aplicação
A aplicação é um site de gerenciamento de campeonatos e-sports, permitindo que os usuários registrem partidas, visualizem informações sobre campeonatos e jogadores.
A aplicação envolve as seguintes entidades principais:

Partida: Registra detalhes sobre partidas específicas, como duração, mapas e campeonato pertencente.

Campeonato: Permite a criação e gerenciamento de campeonatos. Os usuários podem registrar campeonatos, deletar campeonatos, atualizar dados do campeonato e observar informações sobre os campeonatos.

Jogador: As informações sobre jogadores podem ser registradas e associadas aos times participantes dos campeonatos.

Time: Permite a manipulação (adição, remoção e atualização) dos dados do time, como: nome do time, treinador do time, campeonato associado e chave ID

Jogo: O relacionamento jogo mostra o ID da partida e o jogador participante da partida

Pré-requisitos
Antes de começar, certifique-se de ter o seguinte instalado em sua máquina:
Node.js - para executar o servidor
POSTGRESQL - para o banco de dados
VSCode

Passos
1. Configurar o Banco de Dados
Na pasta database, você encontrará os scripts SQL necessários para criar as tabelas do banco de dados. Execute esses scripts no seu servidor POSTGRESQL para criar o esquema do banco de dados.

2. Configurar o Servidor
Abra o arquivo api/server/server.js em um terminal.
Modifique as configurações de conexão com o banco de dados para corresponder às suas credenciais de POSTGRESQL:

javascript
const dbConfig = {  
  user: 'seu_usuario',  
  password: 'sua_senha',  
  host: 'localhost', //local host  
  port: 5432, //sua porta  
  database: 'seu_banco_de_dados'  
};

4. Iniciar o Servidor
Abra o terminal na pasta api do projeto.
Instale as dependências do servidor (encontradas em "./api/package.json") executando o seguinte comando:
npm install {dependencia}
Após a instalação das dependências, inicie o servidor com o seguinte comando:
"nodemon server"

5. Executar o Frontend
Abra o terminal na pasta frontend do projeto.
Inicie um servidor local para o frontend (você pode usar o Live Server se estiver usando o Visual Studio Code) ou abra diretamente o arquivo frontend/index.html em um navegador.

6. Informações dos Integrantes do Grupo:
Luis Guilherme Godim da Fonseca - luis.fonseca@aluno.ufop.edu.br  
João Vitor Tacchi Martins Lanna - joao.tacchi@aluno.ufop.edu.br  
Carlos Henrique Brambati Gomes Sobrinho - carlos.brambati@aluno.ufop.edu.br  
Arthur Alves de Souza - arthur.as1@aluno.ufop.edu.br  
Estevão da Silva Pinto - estevão.pinto@aluno.ufop.edu.br  

Link para repositório no GitHub: https://github.com/joaotacchi1/Trabalho-Pratico-BDno  
Link para mapeamento ER - Relacional: https://drive.google.com/file/d/1eEaD18gXbRVpTAaV9Fx3fvaffosDt4Or/view?usp=sharing  
Link para modelo ER - https://drive.google.com/file/d/1H84nLpQn2_Z-SxUrK4K57aPMEO-qHPPK/view?usp=sharing  
