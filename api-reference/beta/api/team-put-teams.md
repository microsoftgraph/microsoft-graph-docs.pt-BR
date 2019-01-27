---
title: Criar equipe a partir do grupo
description: Crie uma nova equipe a partir de um grupo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a28036cfb253405fab55eca80fa2b0a17232a96c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524790"
---
# <a name="create-team-from-group"></a><span data-ttu-id="bcec4-103">Criar equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="bcec4-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcec4-104">Crie uma nova [equipe](../resources/team.md) a partir de um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="bcec4-104">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="bcec4-105">Para criar uma equipe, o grupo deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="bcec4-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="bcec4-106">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="bcec4-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="bcec4-107">O padrão recomendado é repetir a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="bcec4-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcec4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcec4-108">Permissions</span></span>

<span data-ttu-id="bcec4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcec4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcec4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcec4-111">Permission type</span></span>      | <span data-ttu-id="bcec4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcec4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcec4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcec4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bcec4-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcec4-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcec4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcec4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcec4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcec4-116">Not supported.</span></span>    |
|<span data-ttu-id="bcec4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcec4-117">Application</span></span> | <span data-ttu-id="bcec4-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcec4-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="bcec4-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="bcec4-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bcec4-120">Os administradores globais e administradores do serviço do Microsoft Teams podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="bcec4-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bcec4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcec4-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="bcec4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcec4-122">Request headers</span></span>

| <span data-ttu-id="bcec4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcec4-123">Header</span></span>       | <span data-ttu-id="bcec4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="bcec4-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcec4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcec4-125">Authorization</span></span>  | <span data-ttu-id="bcec4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcec4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bcec4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcec4-128">Content-Type</span></span>  | <span data-ttu-id="bcec4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bcec4-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcec4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcec4-130">Request body</span></span>

<span data-ttu-id="bcec4-131">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bcec4-131">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcec4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcec4-132">Response</span></span>

<span data-ttu-id="bcec4-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcec4-133">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcec4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcec4-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bcec4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcec4-135">Request</span></span>

<span data-ttu-id="bcec4-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcec4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/beta/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```

#### <a name="response"></a><span data-ttu-id="bcec4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcec4-137">Response</span></span>

<span data-ttu-id="bcec4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcec4-138">The following is an example of the response.</span></span> 

><span data-ttu-id="bcec4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcec4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-teams.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="bcec4-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="bcec4-141">See also</span></span>

- [<span data-ttu-id="bcec4-142">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="bcec4-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
