---
title: Criar equipes e gerenciar membros usando o Microsoft Graph
description: 'Criar um grupo que inclui uma equipe envolve as seguintes etapas: '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 80779619006da786652fa02f9d041975e4909e27
ms.sourcegitcommit: fadf83089455674ee721c22d59f7d54758d21896
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2020
ms.locfileid: "43148256"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a>Criar equipes e gerenciar membros usando o Microsoft Graph

Você pode usar a API do Microsoft Teams no Microsoft Graph para criar equipes de várias maneiras. Este artigo descreve a abordagem que recomendamos para obter os melhores resultados.


## <a name="initial-team-creation"></a>Criação da equipe inicial

Todas as equipes têm o suporte de grupos do Office 365. A maneira mais rápida de configurar e utilizar sua equipe ao criar novas equipes através do Microsoft Graph é configurar um novo grupo do Office 365, todos os proprietários e membros e convertê-los em uma equipe.

1. Criar um [grupo do Office 365](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) usando a operação [criar grupo](/graph/api/group-post-groups?view=graph-rest-1.0). Você pode especificar os proprietários e os membros. Certifique-se de que tenha os proprietários certos do grupo recém-criado, conforme descrito na Etapa 2.

    Para criar uma equipe para esse grupo, é necessário definir os seguintes valores de propriedade, conforme mostrado:

    - **groupTypes** = { "Unified" } 
    - **mailEnabled** = true
    - **securityEnabled** = false

    ```http
    POST /groups
    {
        "displayName":"Flight 157",
        "mailNickname":"flight157",
        "description":"Everything about flight 157",
        "visibility":"Private",
        "groupTypes":["Unified"],
        "mailEnabled":true,
        "securityEnabled":false,
        "members@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
            "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
        ],
        "owners@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
        ]
    }
    ```

    O exemplo a seguir mostra a resposta. 

    >**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. Todas as propriedades serão retornadas de uma chamada real.

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. Certifique-se de que o grupo tenha dois ou mais proprietários. É possível fazer isso por meio da operação [adicionar proprietário](/graph/api/group-post-owners?view=graph-rest-1.0). Elas devem ser contas de usuários reais e não contas de serviço. Ter dois proprietários ajuda a lidar com casos em que um proprietário sai da empresa ou não está disponível para realizar operações de gerenciamento de equipe.

3. Adicione todos os membros (e convidados, se necessário) ao grupo usando a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0), caso não tenha feito isso na Etapa 1.

4. Depois que o grupo for criado com êxito, o que pode levar até 15 minutos após concluir a Etapa 1, crie uma equipe do Microsoft Teams usando a operação [criar equipe a partir do grupo](/graph/api/team-post?view=graph-rest-beta#example-4-create-a-team-from-group). Se houver um erro, o processo de criação de grupo pode não ser concluído, tente esperar alguns minutos. 

    ```http
    POST https://graph.microsoft.com/beta/teams
    Content-Type: application/json
    {
      "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
      "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
    }
    ```

    O exemplo a seguir mostra a resposta. 

    >**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. Todas as propriedades serão retornadas de uma chamada real.

    ```http
    HTTP/1.1 202 Accepted
    Content-Type: application/json
    Location: /teams/{teamId}/operations/{operationId}
    Content-Location: /teams/{teamId}
    {
    }
    ```

    A equipe criada tem a mesma ID do que o grupo.

5. Após concluir o processo, todos os proprietários e membros poderão ver a equipe recém-criada no cliente do Teams.

## <a name="adding-or-managing-members"></a>Adicionar ou gerenciar membros

Para adicionar membros depois de criar uma equipe, use a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0). Observe o seguinte em relação às alterações de associação:

1. As alterações de associação aplicadas ao grupos do Office 365 sincronizam com o Teams por meio de um mecanismo de sincronização em segundo plano que geralmente leva 24 horas (ou mais em alguns casos).

2. O processo em segundo plano será acionado somente se um ou mais usuários na equipe (proprietário ou membro) estiverem ativos no cliente da área de trabalho do Teams. A inicialização do aplicativo Teams e/ou sua execução constitui atividade. Um usuário não precisa visitar especificamente a equipe que está sendo modificada.

    >**Observação:** os clientes móveis do Teams não acionam a sincronização de associações. Pelo menos um usuário deve estar no cliente da área de trabalho para garantir que o processo em segundo plano corra bem.

## <a name="checklist-for-validation"></a>Lista de verificação para validação

Depois de criar uma equipe, você pode usar a lista de verificação a seguir para verificar se a equipe foi criada com êxito.

### <a name="validate-team-creation"></a>Validar a criação de equipe

1. Verifique se o grupo do Office 365 que reforça a equipe foi criado por meio do Azure AD ou do centro de administração do Microsoft 365.

2. Verifique se a criação da equipe foi bem-sucedida por meio do portal de administração do Teams.

3. Verifique se a equipe possui os proprietários e membros corretos listados por meio do portal de administração do Teams.

4. Verifique se os proprietários da equipe conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.

5. Verifique se os membros conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.

### <a name="validate-addition-of-members"></a>Validar a adição de membros

1. Verifique se os novos membros aparecem no grupo por meio do Azure AD ou do centro de administração do Microsoft 365.

2. Verifique se os membros recém-adicionados conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.



## <a name="how-office-365-group-membership-changes-are-synchronized-to-microsoft-teams"></a>Como as alterações de associação de grupo do Office 365 são sincronizadas com o Microsoft Teams.

As alterações de associação feitas em grupo do Office 365 que reforça uma equipe por meio da API do Microsoft Graph ou através do portal de administração (fora do cliente do Teams) devem ser sincronizadas com o serviço do Teams para que os usuários recém-adicionados possam ver e participar da equipe. As alterações feitas diretamente à associação de grupo são sincronizadas com o serviço do Teams por meio de um processo em segundo plano. Esse processo em segundo plano é executado no serviço do Teams e é acionado pela atividade do usuário nos clientes da Web e da área de trabalho do Teams.

Para que o processo seja acionado, um proprietário ou membro atual da equipe (alguém que consiga ver a equipe no cliente do Teams) deve estar com o cliente da área de trabalho (ideal) ou da Web aberto. Os clientes móveis não acionam essa sincronização.

O SLA atual para sincronizar as alterações de associação aplicada aos grupos no Teams é de até 24 horas após a sincronização ser acionada por atividade do cliente. Pode levar mais tempo em determinadas circunstâncias (devido à carga do serviço, por exemplo).


![Processo de sincronização da lista de participação.](images/teams-roster-sync.png)

