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
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="c1f22-103">Criar um grupo com uma equipe do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c1f22-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="c1f22-104">A criação de um [grupo](/graph/api/resources/group?view=graph-rest-beta) que inclui uma [equipe](/graph/api/resources/team?view=graph-rest-beta) envolve duas etapas:</span><span class="sxs-lookup"><span data-stu-id="c1f22-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="c1f22-105">[Criar um grupo](/graph/api/group-post-groups?view=graph-rest-beta) com as propriedades certas.</span><span class="sxs-lookup"><span data-stu-id="c1f22-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="c1f22-106">[Adicionar uma equipe](/graph/api/team-put-teams?view=graph-rest-beta) ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c1f22-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="c1f22-107">Criar um grupo</span><span class="sxs-lookup"><span data-stu-id="c1f22-107">Create a group</span></span>

<span data-ttu-id="c1f22-108">Para incluir uma equipe, você precisa definir os seguintes valores de propriedade, conforme mostra o exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="c1f22-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="c1f22-109">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="c1f22-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="c1f22-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="c1f22-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="c1f22-111">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="c1f22-111">**securityEnabled** = false</span></span>

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

<span data-ttu-id="c1f22-112">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1f22-112">The following example shows response.</span></span> 

><span data-ttu-id="c1f22-113">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1f22-113">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="c1f22-114">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1f22-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="c1f22-115">Adicionar uma equipe ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c1f22-115">Add a team to the group</span></span>

<span data-ttu-id="c1f22-116">Adicione uma equipe ao grupo, conforme exibido.</span><span class="sxs-lookup"><span data-stu-id="c1f22-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="c1f22-117">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1f22-117">The following example shows the response.</span></span> 

><span data-ttu-id="c1f22-118">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1f22-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="c1f22-119">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1f22-119">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="c1f22-120">A equipe criada tem a mesma ID do que o grupo.</span><span class="sxs-lookup"><span data-stu-id="c1f22-120">The created team has the same ID as the group.</span></span>
