---
title: Criar equipe
description: Crie uma nova equipe em um grupo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 85a351c3e7ecc276666b6ed912828828de756834
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845693"
---
# <a name="create-team"></a><span data-ttu-id="fe3ef-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="fe3ef-103">Create team</span></span>

<span data-ttu-id="fe3ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe3ef-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="fe3ef-105">Criar uma nova [equipe](../resources/team.md) em um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="fe3ef-105">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="fe3ef-106">Para criar uma equipe, o grupo deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-106">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="fe3ef-107">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-107">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="fe3ef-108">O padrão recomendado é repetir a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-108">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe3ef-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe3ef-109">Permissions</span></span>

<span data-ttu-id="fe3ef-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fe3ef-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe3ef-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe3ef-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe3ef-112">Permission type</span></span>      | <span data-ttu-id="fe3ef-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe3ef-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe3ef-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe3ef-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fe3ef-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3ef-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="fe3ef-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe3ef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe3ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-117">Not supported.</span></span>    |
|<span data-ttu-id="fe3ef-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe3ef-118">Application</span></span> | <span data-ttu-id="fe3ef-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3ef-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="fe3ef-120">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fe3ef-121">Os administradores globais e administradores do serviço do Microsoft Teams podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-121">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe3ef-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe3ef-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="fe3ef-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe3ef-123">Request headers</span></span>

| <span data-ttu-id="fe3ef-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe3ef-124">Header</span></span>       | <span data-ttu-id="fe3ef-125">Valor</span><span class="sxs-lookup"><span data-stu-id="fe3ef-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe3ef-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe3ef-126">Authorization</span></span>  | <span data-ttu-id="fe3ef-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-127">Bearer {token}.</span></span> <span data-ttu-id="fe3ef-128">Required.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-128">Required.</span></span>  |
| <span data-ttu-id="fe3ef-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe3ef-129">Content-Type</span></span>  | <span data-ttu-id="fe3ef-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fe3ef-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe3ef-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe3ef-131">Request body</span></span>

<span data-ttu-id="fe3ef-132">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fe3ef-132">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fe3ef-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe3ef-133">Response</span></span>

<span data-ttu-id="fe3ef-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-134">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe3ef-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe3ef-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fe3ef-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe3ef-136">Request</span></span>

<span data-ttu-id="fe3ef-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe3ef-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe3ef-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreatePrivateChannels": true,
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
# <a name="c"></a>[<span data-ttu-id="fe3ef-139">C#</span><span class="sxs-lookup"><span data-stu-id="fe3ef-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe3ef-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe3ef-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe3ef-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe3ef-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe3ef-142">Java</span><span class="sxs-lookup"><span data-stu-id="fe3ef-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fe3ef-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe3ef-143">Response</span></span>

<span data-ttu-id="fe3ef-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-144">The following is an example of the response.</span></span> 

><span data-ttu-id="fe3ef-145">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe3ef-146">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fe3ef-146">All the properties will be returned from an actual call.</span></span>
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="fe3ef-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="fe3ef-147">See also</span></span>

- [<span data-ttu-id="fe3ef-148">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="fe3ef-148">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
