# DIO - Configurando uma instância de Banco de Dados na Azure
Configurando uma instância de Banco de Dados básico na Azure


## 🔎 Tipos de Serviço de Nuvem	

> Os três tipos de serviço de nuvem oferecidos pela Azure são: IaaS (infraestrutura como serviço), PaaS (plataforma como serviço) e SaaS (software como serviço). Em um modelo de *IaaS*, o provedor de nuvem é responsável por manter o hardware, a conectividade de rede e a segurança física. O cliente é responsável por todo o resto: instalação, configuração e manutenção do sistema operacional; configuração de rede; configuração de banco de dados e armazenamento. Em um ambiente de *PaaS*, o provedor de nuvem mantém a infraestrutura física, a segurança física, a conexão com a Internet, os sistemas operacionais, o middleware, as ferramentas de desenvolvimento e os serviços de business intelligence que compõem uma solução de nuvem. Em um cenário de PaaS, o cliente não precisa se preocupar com o licenciamento nem com a aplicação de patch em sistemas operacionais e bancos de dados. O *SaaS* é o modelo de serviço de nuvem mais completo do ponto de vista do produto. Com o SaaS, o cliente está essencialmente alugando ou usando um aplicativo totalmente desenvolvido, como por exemplo: Email, software financeiro, aplicativos de mensagens e software de conectividade.

<sub>Fonte: - <https://learn.microsoft.com/pt-br/training/modules/describe-cloud-service-types/2-describe-infrastructure-service>
            - <https://learn.microsoft.com/pt-br/training/modules/describe-cloud-service-types/3-describe-platform-service>
            - <https://learn.microsoft.com/pt-br/training/modules/describe-cloud-service-types/4-describe-software-service></sub>


## Criação do Banco de Dados na Azure

Abra o portal da [`Azure`](https://portal.azure.com), clique em **Bancos de Dados SQL** no menu lateral do portal, ou apenas aguarde o menu se expandir e clique em **+ Criar**.

![AZ03-10](https://github.com/user-attachments/assets/23baf57f-d4b3-4327-9372-a597502e2d0b)

Na próxima tela preencha os campos do grupo **Detalhes do projeto**.

![AZ03-03](https://github.com/user-attachments/assets/dfd243fe-036c-49ff-b28e-dce7968ba37f)

![AZ03-11](https://github.com/user-attachments/assets/b2a6fabe-1d2b-4ac4-9ee0-d66c1ecb3144)

Após preencha os campos do grupo **Detalhes do banco de dados**

![AZ03-12](https://github.com/user-attachments/assets/00b8cf77-a4ad-4743-8056-4d9b4038bbf3)

Nesta etapa será necessário criar um novo **Servidor** para o banco de dados.

![AZ03-05](https://github.com/user-attachments/assets/e5b40c2b-a153-4df5-bec6-7901f5cf4120)

Selecione o método de autenticação e clique em **OK**: 

![AZ03-13](https://github.com/user-attachments/assets/73d694e7-8c70-4eac-a704-3213ad76218b)

Pesquise pela conta do Microsoft Entra ID que será utilizada e clique em **Selecionar**:

![AZ03-14](https://github.com/user-attachments/assets/9c3983e2-0952-4854-9fd0-81f6ece1c2ea)

Ao retornar para a página de configuração do Servidor clique em **OK**:

![AZ03-15](https://github.com/user-attachments/assets/5e67a1b4-7642-4d98-8810-89ded1514fd2)

De volta à página de configuração do Banco de dados, repare que o campo do servidor foi preenchido com o servidor que acabamos de criar:

![AZ03-16](https://github.com/user-attachments/assets/7beea34e-9875-4110-a03b-f5928ab7c52f)

Repare que na **Redundância do armazenamento de backup** foi automaticamente selecionada a opção *Armazenamento de backup com redundância geográfica*, podendo ser alterada a opção:

![AZ03-17](https://github.com/user-attachments/assets/20173d4b-bf0d-4f6a-bbff-0fd450937204)

Ao final da página de configuração do banco de dados, é demonstrada uma prévia do valor a ser pago:

![AZ03-09](https://github.com/user-attachments/assets/bdddad5c-17b1-4bc1-a8e0-425f20ec4358)

Para finalizar a criação do banco de dados basta clicar na opção **Revisar + criar** e aguardar a finalização do processo.


## Links utilizados

- https://learn.microsoft.com/pt-br/training/modules/describe-cloud-service-types/2-describe-infrastructure-service

- https://learn.microsoft.com/pt-br/training/modules/describe-cloud-service-types/3-describe-platform-service

- https://learn.microsoft.com/pt-br/training/modules/describe-cloud-service-types/4-describe-software-service

- https://portal.azure.com/#browse/Microsoft.Sql%2Fservers%2Fdatabases
