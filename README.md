Repositório Frontend (Next.js)
Passos para Configurar e Rodar o Projeto
Clone o repositório:
bash
Copiar código
git clone <url-do-repositorio-nextjs>
cd <nome-do-repositorio>
Instale as dependências:
bash
Copiar código
npm install
Configure as variáveis de ambiente:
Crie um arquivo .env.local na raiz do projeto com a variável NEXT_PUBLIC_API_URL apontando para a URL da API Laravel.
Exemplo:
env
Copiar código
NEXT_PUBLIC_API_URL=http://localhost:8000/api
Inicie o servidor de desenvolvimento:
bash
Copiar código
npm run dev
Acesse a aplicação no navegador em http://localhost:3000.
Explicação sobre a Funcionalidade Implementada
O frontend fornece uma interface para o cadastro de profissões.
Inclui um formulário com os seguintes campos:
Nome (obrigatório)
Descrição (opcional)
Salário (obrigatório)
Empresa (obrigatório)
Ao enviar o formulário, os dados são enviados para a API Laravel via método POST.
Descrição do Fluxo de Dados
O usuário preenche o formulário no frontend.
Os dados são validados localmente (se necessário) e enviados para a API do backend usando o método POST.
O backend armazena os dados na base de dados e retorna uma resposta ao frontend.
O frontend exibe mensagens de sucesso ou erro com base na resposta.
