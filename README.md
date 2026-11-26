Recicle Aqui
Aplicação web para mapeamento e gestão de pontos de coleta seletiva e reciclagem.

Como executar o projeto localmente
Pré-requisitos
Node.js instalado

Git Bash (ou terminal compatível)

Conta/projeto configurado no Supabase

Passo a passo

Clone o repositório e abra no VS Code:

cmd 
git clone <URL_DO_REPOSITORIO>
cd <RecicleAqui_corrigido>
code .
Abra o terminal (Git Bash) no VS Code e acesse a pasta do backend:

Bash
cd recicleaqui

Instale as dependências:

Bash
npm install
npm install --legacy-peer-deps

Crie o arquivo de variáveis de ambiente:

Bash
touch .env
code .env


Configure as variáveis:

Copie todo o conteúdo do arquivo exemplo.env.
(SUPABASE_URL=https://othkpmvxeznveaagqhbm.supabase.co
SUPABASE_SERVICE_ROLE_KEY=sb_secret_4JqYWlqIcZjQfMAWnDlDww_KepK2NVF
SUPABASE_PUBLISHABLE_KEY=sb_publishable_dwhXNA_3oVazgopxQeu69Q_2o24lpGj
JWT_SECRET=qualquer-segredo-grande-aqui
OWNER_OPEN_ID=
NODE_ENV=development
PORT=3000)

Cole dentro do arquivo .env que você acabou de abrir e preencha com as credenciais do seu Supabase.

Salve o arquivo (Ctrl + S).

Inicie o servidor de desenvolvimento:

Bash
npm run dev
Acesse a aplicação no navegador pelo endereço exibido no terminal (geralmente http://localhost:3000 ou http://localhost:5173).