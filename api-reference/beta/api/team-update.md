---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6915b3f4409e5d4948cd02c7a5540821ffb0928
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452565"
---
# <a name="update-team"></a><span data-ttu-id="18634-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="18634-103">Update team</span></span>

<span data-ttu-id="18634-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="18634-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18634-105">Atualize as propriedades da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="18634-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18634-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18634-106">Permissions</span></span>
<span data-ttu-id="18634-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="18634-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18634-109">Permission type</span></span>      | <span data-ttu-id="18634-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18634-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18634-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18634-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18634-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18634-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18634-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18634-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18634-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18634-114">Not supported.</span></span>    |
|<span data-ttu-id="18634-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18634-115">Application</span></span> | <span data-ttu-id="18634-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18634-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="18634-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="18634-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18634-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="18634-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18634-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18634-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="18634-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18634-120">Request headers</span></span>
| <span data-ttu-id="18634-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18634-121">Header</span></span>       | <span data-ttu-id="18634-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18634-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18634-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18634-123">Authorization</span></span>  | <span data-ttu-id="18634-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18634-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18634-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18634-126">Content-Type</span></span>  | <span data-ttu-id="18634-127">application/json</span><span class="sxs-lookup"><span data-stu-id="18634-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18634-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18634-128">Request body</span></span>
<span data-ttu-id="18634-129">No corpo da solicitação, forneça uma representação JSON do objeto [Team](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="18634-129">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18634-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="18634-130">Response</span></span>

<span data-ttu-id="18634-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="18634-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18634-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18634-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="18634-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18634-133">Request</span></span>
<span data-ttu-id="18634-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18634-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18634-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="18634-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

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
# <a name="javascript"></a>[<span data-ttu-id="18634-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18634-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="18634-137">C#</span><span class="sxs-lookup"><span data-stu-id="18634-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18634-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18634-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="18634-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="18634-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
