---
title: Listar todas as equipes do Microsoft Teams para uma organização
description: 'Listar todas as equipes '
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 6a1c4a19900263460bdd1f282cd87aee45ec7af7
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118526"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>Listar todas as equipes do Microsoft Teams para uma organização

Para listar todas as [equipes](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) em uma organização (locatário), você deve localizar todos os grupos que possuem equipes e, em seguida, obter informações de cada equipe.

## <a name="get-a-list-of-groups"></a>Obter uma lista de grupos

#### <a name="example-1-get-list-of-groups-that-contain-a-team"></a>Exemplo 1: Obter lista de grupos que contêm uma equipe
Para obter uma lista de todos os [grupos](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) da organização que possuem equipes, obtenha uma [lista de todos os grupos](/graph/api/group-list?view=graph-rest-1.0&preserve-view=true) e depois, em código, localize os que têm a propriedade **resourceProvisioningOptions** que contém “Equipe”.

Use a API com `$filter` para retornar apenas os grupos que têm equipes.

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> **Observação**: certas equipes antigas não utilizadas não terão a configuração **resourceProvisioningOptions**. Para saber mais, confira [problemas conhecidos](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined).

Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. 
>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "02bd9fd6-8f93-4758-87c3-1fb73740a315",
            "description": "Welcome to the HR Taskforce team.",
            "displayName": "HR Taskforce",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "HRTaskforce",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private"
        },
        {
            "id": "8090c93e-ba7c-433e-9f39-08c7ba07c0b3",
            "description": "Welcome to the team that we've assembled to launch our product.",
            "displayName": "X1050 Launch Team",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "X1050LaunchTeam",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private"
        }
    ]
}
```

#### <a name="example-2-get-list-of-groups-by-selecting-required-properties-only"></a>Exemplo 2: obter lista de grupos selecionando apenas as propriedades necessárias
Como os grupos são objetos grandes, use `$select` para obter as propriedades apenas do grupo que importa para você.

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> **Observação**: certas equipes antigas não utilizadas não terão a configuração **resourceProvisioningOptions**. Para saber mais, confira [problemas conhecidos](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined).

Este é um exemplo de resposta. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "00e897b1-70ba-4cb9-9126-fd5f95c4bb78",
            "resourceProvisioningOptions": []
        },
        {
            "id": "00f6e045-f884-4359-a617-d459ee626862",
            "resourceProvisioningOptions": [
                "Team"
            ]
        }
    ]
}

```

## <a name="get-team-information-for-a-group"></a>Obter informações de equipe para um grupo

Para obter informações de equipe para a equipe de um grupo específico, chame a API [get team](/graph/api/team-get?view=graph-rest-1.0&preserve-view=true) e incluam a ID do grupo.

```http
GET /teams/{group-id}
```

O exemplo a seguir mostra a resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

## <a name="see-also"></a>Confira também

- [Listar joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true)
- [Listar grupos](/graph/api/group-list?view=graph-rest-1.0&preserve-view=true)
