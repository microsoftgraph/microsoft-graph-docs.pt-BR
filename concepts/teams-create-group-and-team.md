---
title: Criar um grupo com uma equipe do Microsoft Teams
description: 'A criação de um grupo que inclui uma equipe envolve duas etapas: '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 06b25a6da159030407c904622ffebde09c704d98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970476"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>Criar um grupo com uma equipe do Microsoft Teams

A criação de um [grupo](/graph/api/resources/group?view=graph-rest-beta) que inclui uma [equipe](/graph/api/resources/team?view=graph-rest-beta) envolve duas etapas: 

- [Criar um grupo](/graph/api/group-post-groups?view=graph-rest-beta) com as propriedades certas.
- [Adicionar uma equipe](/graph/api/team-put-teams?view=graph-rest-beta) ao grupo.

## <a name="create-a-group"></a>Criar um grupo

Para incluir uma equipe, você precisa definir os seguintes valores de propriedade, conforme mostra o exemplo a seguir:

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

## <a name="add-a-team-to-the-group"></a>Adicionar uma equipe ao grupo.

Adicione uma equipe ao grupo, conforme exibido.

```http
PUT /groups/{id}/team
{ }
```

O exemplo a seguir mostra a resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
    "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
    "webUrl" : "https://example.com",
    "isArchived" : null,
    "memberSettings" : { },
    "guestSettings" : { },
    "messagingSettings" : { },
    "funSettings" : {}
}
```

A equipe criada tem a mesma ID do que o grupo.
