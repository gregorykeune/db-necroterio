# Banco de Dados de Necrotério

Este projeto contém o modelo lógico de um sistema de banco de dados para gerenciamento de um necrotério. O sistema é voltado para o controle de informações de falecidos, funcionários, documentos, entradas e saídas, além do destino dos corpos e vínculos com encarregados.

## Objetivo

O sistema visa fornecer uma estrutura robusta e organizada para armazenar e consultar informações relacionadas à operação de um necrotério, incluindo:

- Registro de falecidos
- Funcionários e seus cargos
- Entrada e saída de corpos
- Encaminhamento para funerárias
- Documentação associada
- Relação com dependentes e encarregados

---

## Modelo Lógico

O banco de dados é composto pelas seguintes principais tabelas:

### `tb_falecido`
Armazena dados dos falecidos, como nome, data e local do falecimento, documentos, e endereço.

### `tb_pessoas`
Contém informações de pessoas relacionadas ao necrotério (familiares, responsáveis, etc).

### `tb_destino_corpo`
Registra os dados das funerárias para onde os corpos são encaminhados.

### `tb_encarregado`
Define quem são os responsáveis legais pelos falecidos.

### `tb_funcionario`
Registra os funcionários do necrotério, com vínculos a permissões, cargos e documentos.

### `tb_permissao`
Controla o nível de acesso de cada funcionário.

### `tb_funcao` e `tb_departamento`
Definem a função e o departamento de cada funcionário.

### `tb_corporacao`
Armazena dados da empresa ou instituição que opera o necrotério.

### `tb_dependente`
Relaciona os dependentes dos funcionários.

### `tb_entrada_saida`
Registra os horários de entrada e saída de corpos.

### `tb_documento` e `tb_funcionario_possui_doc`
Controlam os documentos associados a falecidos e funcionários.

---

## 🛠️ Tecnologias Utilizadas

- **MySQL Workbench** — modelagem do banco de dados
- **MySQL** — sistema gerenciador de banco de dados relacional
