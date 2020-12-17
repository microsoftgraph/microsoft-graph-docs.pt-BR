---
title: Criar equipe a partir do grupo
description: Crie uma nova equipe a partir de um grupo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f17d6db22e2076b66d62453da900216a55a899ef
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977434"
---
# <a name="create-team-from-group"></a><span data-ttu-id="ef1b0-103">Criar equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="ef1b0-103">Create team from group</span></span>

<span data-ttu-id="ef1b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef1b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> <span data-ttu-id="ef1b0-105">Essa API está sendo preterida em favor de [Criar equipe](../api/team-post.md) e será removida até o final de 2019.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-105">This API is in the process of being deprecated in favor of [Create team](../api/team-post.md), and will be removed by the end of 2019.</span></span> <span data-ttu-id="ef1b0-106">Para obter detalhes sobre como criar uma equipe a partir de um grupo, confira os exemplos 4 e 5 em [Criar equipe](../api/team-post.md).</span><span class="sxs-lookup"><span data-stu-id="ef1b0-106">For details about how to create a team from a group, see examples 4 and 5 in [Create team](../api/team-post.md).</span></span>

<span data-ttu-id="ef1b0-107">Crie uma nova [equipe](../resources/team.md) a partir de um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="ef1b0-107">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="ef1b0-108">Para criar uma equipe, o grupo deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-108">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="ef1b0-109">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-109">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="ef1b0-110">O padrão recomendado é repetir a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-110">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef1b0-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef1b0-111">Permissions</span></span>

<span data-ttu-id="ef1b0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef1b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef1b0-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef1b0-114">Permission type</span></span>      | <span data-ttu-id="ef1b0-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef1b0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef1b0-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef1b0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ef1b0-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1b0-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ef1b0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef1b0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1b0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-119">Not supported.</span></span>    |
|<span data-ttu-id="ef1b0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef1b0-120">Application</span></span> | <span data-ttu-id="ef1b0-121">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1b0-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ef1b0-122">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ef1b0-123">Os administradores globais e administradores do serviço do Microsoft Teams podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-123">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ef1b0-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef1b0-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="ef1b0-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1b0-125">Request headers</span></span>

| <span data-ttu-id="ef1b0-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef1b0-126">Header</span></span>       | <span data-ttu-id="ef1b0-127">Valor</span><span class="sxs-lookup"><span data-stu-id="ef1b0-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef1b0-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef1b0-128">Authorization</span></span>  | <span data-ttu-id="ef1b0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef1b0-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef1b0-131">Content-Type</span></span>  | <span data-ttu-id="ef1b0-132">application/json</span><span class="sxs-lookup"><span data-stu-id="ef1b0-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef1b0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1b0-133">Request body</span></span>

<span data-ttu-id="ef1b0-134">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ef1b0-134">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef1b0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef1b0-135">Response</span></span>

<span data-ttu-id="ef1b0-136">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-136">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef1b0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef1b0-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ef1b0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1b0-138">Request</span></span>

<span data-ttu-id="ef1b0-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef1b0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef1b0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ef1b0-141">C#</span><span class="sxs-lookup"><span data-stu-id="ef1b0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef1b0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef1b0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef1b0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef1b0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef1b0-144">Java</span><span class="sxs-lookup"><span data-stu-id="ef1b0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef1b0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef1b0-145">Response</span></span>

<span data-ttu-id="ef1b0-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-146">The following is an example of the response.</span></span> 

><span data-ttu-id="ef1b0-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef1b0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
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
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="ef1b0-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="ef1b0-149">See also</span></span>

- [<span data-ttu-id="ef1b0-150">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="ef1b0-150">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)


