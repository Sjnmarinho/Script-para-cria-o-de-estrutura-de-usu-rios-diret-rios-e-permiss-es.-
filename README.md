📖 Sobre o Projeto
Este projeto implementa um script de automação Infrastructure as Code (IaC) para criação automatizada de usuários, grupos e estrutura de diretórios em sistemas Linux. Desenvolvido como parte do desafio do curso Linux Experience da DIO.

🎯 Objetivos
✅ Automatizar a criação de estrutura de usuários e grupos

✅ Implementar política de permissões por departamento

✅ Garantir consistência em múltiplos ambientes

✅ Praticar conceitos de Infrastructure as Code

🏗️ Arquitetura da Solução
Estrutura de Grupos
Grupo	Departamento	Permissões
GRP_ADM	Administração	Acesso total aos sistemas
GRP_VEN	Vendas	Acesso a dados comerciais
GRP_SEC	Secretaria	Acesso a documentos administrativos
Usuários Criados
Usuário	Grupo	Departamento
carlos	GRP_ADM	Administração
maria	GRP_ADM	Administração
joao	GRP_ADM	Administração
debora	GRP_VEN	Vendas
sebastiana	GRP_VEN	Vendas
roberto	GRP_VEN	Vendas
josefina	GRP_SEC	Secretaria
amanda	GRP_SEC	Secretaria
rogerio	GRP_SEC	Secretaria
🚀 Como Usar

Pré-requisitos

  . Sistema Linux
  . Acesso root ou sudo
  . Git (para clonar o repositório)

Execução

1. Clone o repositório:

  git clone https://github.com/Sjnmarinho/Script-para-cria-o-de-estrutura-de-usu-rios-diret-rios-e-permiss-es.-.git

  cd linux-projeto-iac

2. Torne o script executável:

  chmod +x setup_infra.sh

3. Execute como root:

  sudo ./setup_infra.sh

  Execução Direta (uma linha)

  sudo bash -c "$(curl -fsSL https://github.com/Sjnmarinho/Script-para-cria-o-de-estrutura-de-usu-rios-diret-rios-e-permiss-es.-.git)"

📊 Fluxo de Execução

Criação de Diretórios → 2. Criação de Grupos → 3. Criação de Usuários → 4. Configuração de Permissões → 5. Finalização

🛠️ Tecnologias Utilizadas

. Bash Script

. Linux Users & Groups

. Permission Management

. OpenSSL (para geração de senhas)

  Bons estudos !
