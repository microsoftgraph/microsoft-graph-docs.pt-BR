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
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a><span data-ttu-id="a7272-103">Listar todas as equipes do Microsoft Teams para uma organização</span><span class="sxs-lookup"><span data-stu-id="a7272-103">List all teams in Microsoft Teams for an organization</span></span>

<span data-ttu-id="a7272-104">Para listar todas as [equipes](/graph/api/resources/team?view=graph-rest-beta) em uma organização (locatário), você deve localizar todos os grupos que possuem equipes e, em seguida, obter informações de cada equipe.</span><span class="sxs-lookup"><span data-stu-id="a7272-104">To list all [teams](/graph/api/resources/team?view=graph-rest-beta) in an organization (tenant), you find all groups that have teams, and then get information for each team.</span></span>

## <a name="get-a-list-of-groups"></a><span data-ttu-id="a7272-105">Obter uma lista de grupos</span><span class="sxs-lookup"><span data-stu-id="a7272-105">Get a list of groups</span></span>

<span data-ttu-id="a7272-106">Para obter uma lista de todos os [grupos](/graph/api/resources/group?view=graph-rest-beta) da organização que possuem equipes, obtenha uma [lista de todos os grupos](/graph/api/group-list?view=graph-rest-beta) e depois, em código, localize os que têm a propriedade **resourceProvisioningOptions** que contém “Equipe”.</span><span class="sxs-lookup"><span data-stu-id="a7272-106">To get a list of all [groups](/graph/api/resources/group?view=graph-rest-beta) in the organization that have teams, get a [list of all groups](/graph/api/group-list?view=graph-rest-beta) and then in code find the ones that have a **resourceProvisioningOptions** property that contains "Team".</span></span>
<span data-ttu-id="a7272-107">Como os grupos são objetos grandes, use $select para obter as propriedades apenas do grupo que importa para você.</span><span class="sxs-lookup"><span data-stu-id="a7272-107">Since groups are large objects, use $select to only get the properties of the group you care about.</span></span>

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> <span data-ttu-id="a7272-108">**Observação**: certas equipes antigas não utilizadas não terão a configuração resourceProvisioningOptions.</span><span class="sxs-lookup"><span data-stu-id="a7272-108">**Note**: Certain unused old teams will not have resourceProvisioningOptions set.</span></span> <span data-ttu-id="a7272-109">Para saber mais, confira [problemas conhecidos](known-issues.md#missing-teams-in-list-all-teams).</span><span class="sxs-lookup"><span data-stu-id="a7272-109">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="a7272-110">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7272-110">The following is an example of the response.</span></span> 

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

## <a name="get-a-list-of-groups-using-beta-apis"></a><span data-ttu-id="a7272-111">Obter uma lista de grupos usando as APIs beta</span><span class="sxs-lookup"><span data-stu-id="a7272-111">Get a list of groups using beta APIs</span></span>

<span data-ttu-id="a7272-112">Usando as APIs beta, você pode usar $filter para retornar apenas os grupos que possuem equipes.</span><span class="sxs-lookup"><span data-stu-id="a7272-112">Using the beta APIs, you can use $filter to return only the groups that have teams.</span></span>

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> <span data-ttu-id="a7272-113">**Observação**: a filtragem de grupos por resourceProvisioningOptions só está disponível por meio do ponto de extremidade beta.</span><span class="sxs-lookup"><span data-stu-id="a7272-113">**Note**: Filtering groups by resourceProvisioningOptions is only available through the beta endpoint.</span></span> <span data-ttu-id="a7272-114">resourceProvisioningOptions está disponível na versão 1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="a7272-114">resourceProvisioningOptions is available in v1.0 and beta.</span></span>

> <span data-ttu-id="a7272-115">**Observação**: certas equipes antigas não utilizadas não serão listadas.</span><span class="sxs-lookup"><span data-stu-id="a7272-115">**Note**: Certain unused old teams will not be listed.</span></span> <span data-ttu-id="a7272-116">Para saber mais, confira [problemas conhecidos](known-issues.md#missing-teams-in-list-all-teams).</span><span class="sxs-lookup"><span data-stu-id="a7272-116">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="a7272-117">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7272-117">The following is an example of the response.</span></span> 

><span data-ttu-id="a7272-p105">**Observação:** O objeto de resposta mostrado pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7272-p105">**Note:** The response object shown might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="get-team-information-for-a-group"></a><span data-ttu-id="a7272-120">Obter informações de equipe para um grupo</span><span class="sxs-lookup"><span data-stu-id="a7272-120">Get team information for a group</span></span>

<span data-ttu-id="a7272-121">Para obter informações de equipe para a equipe de um grupo específico, chame a API [get team](/graph/api/team-get?view=graph-rest-beta) e incluam a ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="a7272-121">To get team information for the team in a particular group, call the [get team](/graph/api/team-get?view=graph-rest-beta) API and include the group ID.</span></span>

```http
GET /teams/{group-id}
```

<span data-ttu-id="a7272-122">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7272-122">The following example shows the response.</span></span>

><span data-ttu-id="a7272-123">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a7272-123">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a7272-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="a7272-124">See also</span></span>

- [<span data-ttu-id="a7272-125">Listar joinedTeams</span><span class="sxs-lookup"><span data-stu-id="a7272-125">List joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [<span data-ttu-id="a7272-126">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="a7272-126">List groups</span></span>](/graph/api/group-list?view=graph-rest-beta)
