<h1 align="center">
    <br>
    <p align="center"> Implantação de WordPress com Amazon ECS usando AWS CloudFormation 🪄💻 <p>
</h1></br>

<!--ts-->
- [💻 Implantação de WordPress com Amazon ECS usando AWS CloudFormation ](#-Implantação-de-WordPress-com-Amazon-ECS-usando-AWS-CloudFormation)
- [🪄 Passo a Passo ](#-passo-a-passo)

<!--te-->

</br>

# 💻 Implantação de WordPress com Amazon ECS usando AWS CloudFormation

Criou uma pilha do AWS CloudFormation para implantar um ambiente altamente disponível do WordPress usando o Amazon ECS (Elastic Container Service).

O ambiente incluirá um cluster ECS, uma definição de tarefa, um serviço, um balanceador de carga, dimensionamento automático e um sistema de arquivos EFS para armazenar dados persistentes do WordPress.

# 🪄 Passo a Passo:

### 🪄 Repositório:
Crie um Repositório no GitHub: Crie um repositório no GitHub para armazenar todos os artefatos relacionados a este projeto, incluindo o template do CloudFormation e outros arquivos relevantes, lembre-se de escrever um Readme para essa aplicação.

### 🪄 Template:
Defina o Template do CloudFormation: No repositório, crie um arquivo chamado ecs-wordpress-stack.yml (ou outro nome de sua escolha) que conterá o template do CloudFormation. Este arquivo definirá todos os recursos necessários para a infraestrutura.

### 🪄 Infraestrutura:
Descreva a Infraestrutura: No template do CloudFormation, defina os seguintes recursos:

### 🪄 Cluster, Containers, Balanceador e Dimensionamento automático :
Um cluster ECS para hospedar os containers do WordPress.
Uma definição de tarefa que especifica como os containers do WordPress serão configurados.
Um serviço ECS para garantir que a tarefa do WordPress seja sempre executada.
Um balanceador de carga para distribuir o tráfego entre os containers.
Configurações de dimensionamento automático para ajustar automaticamente o número de containers com base na carga.
Um sistema de arquivos EFS para armazenar dados persistentes do WordPress.
Use Parâmetros:

No template, utilize parâmetros para permitir a personalização durante a criação da pilha, como nome do cluster, tamanho da instância, etc.
Documente seu Template: Forneça comentários claros no template para explicar a finalidade de cada recurso e parâmetro.

Implante a Pilha: Implante a pilha através do CLI ou do Management Console, a escolha é livre.

Verifique o Ambiente: Após a conclusão da implantação, verifique se o ambiente do WordPress está funcionando corretamente. Você pode acessar o endereço do balanceador de carga para acessar o WordPress.

### 🪄 Recomendações:
Lembre-se de seguir as práticas recomendadas do CloudFormation, como nomear recursos adequadamente, adicionar descrições claras e aplicar políticas de segurança apropriadas. Esta é uma tarefa complexa, portanto, não hesite em consultar a documentação oficial da AWS para obter orientações detalhadas ao longo do processo.
