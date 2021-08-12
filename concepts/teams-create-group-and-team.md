---
title: Criar equipes e gerenciar membros usando o Microsoft Graph
description: 'Criar um grupo que inclui uma equipe envolve as seguintes etapas: '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 454466aff5a83cd9593c2a87a0c933c8ec7b0a4650d757c6754369f03eea0f4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246371"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a>Criar equipes e gerenciar membros usando o Microsoft Graph

Você pode usar a API do Microsoft Teams no Microsoft Graph para criar equipes de várias maneiras. Este artigo descreve a abordagem que recomendamos para obter os melhores resultados.


## <a name="initial-team-creation"></a>Criação da equipe inicial

Todas as equipes são apoiadas pelo Microsoft 365 groups. A maneira mais rápida de preparar sua equipe ao criar novas equipes por meio do Microsoft Graph é configurar um novo grupo do Microsoft 365, todos os proprietários e membros e convertê-lo em uma equipe.

1. Criar um [grupo do Microsoft 365](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) usando a operação [criar grupo](/graph/api/group-post-groups?view=graph-rest-1.0). Você pode especificar os proprietários e os membros. Certifique-se de que tenha os proprietários certos do grupo recém-criado, conforme descrito na Etapa 2.

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

    >**Observação:** O objeto de resposta mostrado pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.

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

3. Adicione todos os membros (e convidados, se necessário) ao grupo usando a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0), caso não tenha feito isso na Etapa 1. Se você estiver adicionando vários membros, adicione um atraso de 1 segundo após cada operação de adição. 

4. Depois que o grupo for criado com sucesso, o que pode levar até 15 minutos após a conclusão da Etapa 1, crie uma equipe do Microsoft Teams usando a operação [criar equipe a partir de grupo](/graph/api/team-post?view=graph-rest-beta#example-4-create-a-team-from-group). Se houver um erro, o processo de criação de grupo pode não ser concluído, tente esperar alguns minutos. 

    ```http
    POST https://graph.microsoft.com/beta/teams
    Content-Type: application/json
    {
      "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
      "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
    }
    ```

    O exemplo a seguir mostra a resposta. 

    >**Observação:** O objeto de resposta mostrado pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.

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

Para adicionar membros depois de criar uma equipe, use a operação [adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0). É recomendável adicionar um atraso de 1 segundo entre as operações adicionar. Observe o seguinte em relação às alterações de associação:

1. As alterações de associação feitas nos grupos do Microsoft 365 são sincronizadas com o Teams por meio de um mecanismo de sincronização de tela de fundo que geralmente demora 24 horas ou mais, em alguns casos.

2. O processo em segundo plano será acionado somente se um ou mais usuários na equipe (proprietário ou membro) estiverem ativos no cliente da área de trabalho do Teams. A inicialização do aplicativo Teams e/ou sua execução constitui atividade. Um usuário não precisa visitar especificamente a equipe que está sendo modificada.

    >**Observação:** os clientes móveis do Teams não acionam a sincronização de associações. Pelo menos um usuário deve estar no cliente da área de trabalho para garantir que o processo em segundo plano corra bem.

## <a name="checklist-for-validation"></a>Lista de verificação para validação

Depois de criar uma equipe, você pode usar a lista de verificação a seguir para verificar se a equipe foi criada com êxito.

### <a name="validate-team-creation"></a>Validar a criação de equipe

1. Verifique se o grupo do Microsoft 365 que reforça a equipe foi criado por meio do Azure AD ou do centro de administração do Microsoft 365.

2. Verifique se a criação da equipe foi bem-sucedida por meio do portal de administração do Teams.

3. Verifique se a equipe possui os proprietários e membros corretos listados por meio do portal de administração do Teams.

4. Verifique se os proprietários da equipe conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.

5. Verifique se os membros conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.

### <a name="validate-addition-of-members"></a>Validar a adição de membros

1. Verifique se os novos membros aparecem no grupo por meio do Azure AD ou do centro de administração do Microsoft 365.

2. Verifique se os membros recém-adicionados conseguem ver a equipe após entrar no cliente da Web ou da área de trabalho do Teams.
