Script de Automação de Infraestrutura Linux

📋 Descrição do Projeto

Este projeto consiste em um script de automação para criação de infraestrutura de usuários, grupos e diretórios em sistemas Linux. O script segue a metodologia Infrastructure as Code (IaC), permitindo a reprodução consistente do ambiente em qualquer máquina virtual.

🎯 Objetivo

Automatizar a criação de:

. Grupos de usuários por departamento

. Usuários com associação aos respectivos grupos

. Diretórios com permissões específicas

. Estrutura de permissões organizada

🏗️ Estrutura Criada

Grupos

. GRP_ADM  -  Grupo de Administração

. GRP_VEN  -  Grupo de Vendas

. GRP_SEC  -  Grupo de Secretaria

Usuários

Grupo		   Usuários
GRP_ADM		 carlos, maria, joao
GRP_VEN		 debora, sebastiana, roberto
GRP_SEC		 josefina, amanda, rogerio

Diretórios e Permissões

Diretório       Grupo	 Permissões  Descrição
/adm		        GRP_ADM	 770	     Acesso exclusivo para administradores
/ven		        GRP_VEN	 770	     Acesso exclusivo para vendedores
/sec		        GRP_SEC	 770	     Acesso exclusivo para secretárias
/publico	      Todos	   777	     Área de compartilhamento geral

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
