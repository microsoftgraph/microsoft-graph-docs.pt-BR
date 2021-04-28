---
title: Criar equipe a partir do grupo
description: Crie uma nova equipe em um grupo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 11ecce195d6a93d5384f67fef2bb23f6cf34d6c8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051225"
---
# <a name="create-team-from-group"></a><span data-ttu-id="6f150-103">Criar equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="6f150-103">Create team from group</span></span>

<span data-ttu-id="6f150-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f150-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6f150-105">Criar uma nova [equipe](../resources/team.md) em um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="6f150-105">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="6f150-106">Para criar uma equipe, o grupo deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="6f150-106">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="6f150-107">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="6f150-107">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="6f150-108">O padrão recomendado é repetir a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="6f150-108">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f150-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f150-109">Permissions</span></span>

<span data-ttu-id="6f150-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f150-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f150-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f150-112">Permission type</span></span>      | <span data-ttu-id="6f150-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f150-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f150-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f150-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6f150-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f150-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6f150-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f150-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f150-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f150-117">Not supported.</span></span>    |
|<span data-ttu-id="6f150-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f150-118">Application</span></span> | <span data-ttu-id="6f150-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f150-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="6f150-120">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6f150-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6f150-121">Os administradores globais e administradores do serviço do Microsoft Teams podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="6f150-121">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6f150-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f150-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="6f150-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f150-123">Request headers</span></span>

| <span data-ttu-id="6f150-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f150-124">Header</span></span>       | <span data-ttu-id="6f150-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6f150-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6f150-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f150-126">Authorization</span></span>  | <span data-ttu-id="6f150-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f150-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6f150-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f150-129">Content-Type</span></span>  | <span data-ttu-id="6f150-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6f150-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f150-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f150-131">Request body</span></span>

<span data-ttu-id="6f150-132">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="6f150-132">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6f150-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f150-133">Response</span></span>

<span data-ttu-id="6f150-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f150-134">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f150-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f150-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6f150-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f150-136">Request</span></span>

<span data-ttu-id="6f150-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f150-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f150-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f150-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6f150-139">C#</span><span class="sxs-lookup"><span data-stu-id="6f150-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f150-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f150-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f150-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f150-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f150-142">Java</span><span class="sxs-lookup"><span data-stu-id="6f150-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f150-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f150-143">Response</span></span>

<span data-ttu-id="6f150-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f150-144">The following is an example of the response.</span></span> 

><span data-ttu-id="6f150-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f150-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6f150-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="6f150-146">See also</span></span>

- [<span data-ttu-id="6f150-147">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="6f150-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)

