---
title: Listar todas as equipes do Microsoft Teams para uma organização
description: 'Listar todas as equipes '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8bacd936f67c0ba02ba547104eb9a7983017cbe8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051148"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>Listar todas as equipes do Microsoft Teams para uma organização

Para listar todas as [equipes](/graph/api/resources/team?view=graph-rest-beta) em uma organização (locatário), você deve localizar todos os grupos que possuem equipes e, em seguida, obter informações de cada equipe.

## <a name="get-a-list-of-groups"></a>Obter uma lista de grupos

Para obter uma lista de todos os [grupos](/graph/api/resources/group?view=graph-rest-beta) da organização que possuem equipes, obtenha uma [lista de todos os grupos](/graph/api/group-list?view=graph-rest-beta) e depois, em código, localize os que têm a propriedade **resourceProvisioningOptions** que contém “Equipe”.
Como os grupos são objetos grandes, use $select para obter as propriedades apenas do grupo que importa para você.

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> **Observação**: certas equipes antigas não utilizadas não terão a configuração resourceProvisioningOptions. Para saber mais, confira [problemas conhecidos](known-issues.md#missing-teams-in-list-all-teams).

Este é um exemplo de resposta. 

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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

## <a name="get-a-list-of-groups-using-beta-apis"></a>Obter uma lista de grupos usando as APIs beta

Usando as APIs beta, você pode usar $filter para retornar apenas os grupos que possuem equipes.

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> **Observação**: a filtragem de grupos por resourceProvisioningOptions só está disponível por meio do ponto de extremidade beta. resourceProvisioningOptions está disponível na versão 1.0 e beta.

> **Observação**: certas equipes antigas não utilizadas não serão listadas. Para saber mais, confira [problemas conhecidos](known-issues.md#missing-teams-in-list-all-teams).

Este é um exemplo de resposta. 

>**Observação:** O objeto de resposta mostrado pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
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

## <a name="get-team-information-for-a-group"></a>Obter informações de equipe para um grupo

Para obter informações de equipe para a equipe de um grupo específico, chame a API [get team](/graph/api/team-get?view=graph-rest-beta) e incluam a ID do grupo.

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
Content-length: 401

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

- [Listar joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [Listar grupos](/graph/api/group-list?view=graph-rest-beta)
