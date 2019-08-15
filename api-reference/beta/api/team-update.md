---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 325c5d9813794a57b59de6caaaea359d3f51f830
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421327"
---
# <a name="update-team"></a><span data-ttu-id="96a0f-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="96a0f-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96a0f-104">Atualize as propriedades da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="96a0f-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96a0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="96a0f-105">Permissions</span></span>
<span data-ttu-id="96a0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96a0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="96a0f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96a0f-108">Permission type</span></span>      | <span data-ttu-id="96a0f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96a0f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96a0f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96a0f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96a0f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a0f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96a0f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96a0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96a0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96a0f-113">Not supported.</span></span>    |
|<span data-ttu-id="96a0f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96a0f-114">Application</span></span> | <span data-ttu-id="96a0f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a0f-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="96a0f-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="96a0f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="96a0f-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="96a0f-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="96a0f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96a0f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="96a0f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96a0f-119">Request headers</span></span>
| <span data-ttu-id="96a0f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96a0f-120">Header</span></span>       | <span data-ttu-id="96a0f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96a0f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96a0f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96a0f-122">Authorization</span></span>  | <span data-ttu-id="96a0f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96a0f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96a0f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96a0f-125">Content-Type</span></span>  | <span data-ttu-id="96a0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96a0f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96a0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96a0f-127">Request body</span></span>
<span data-ttu-id="96a0f-128">No corpo da solicitação, forneça uma representação JSON do objeto [Team](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="96a0f-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="96a0f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a0f-129">Response</span></span>

<span data-ttu-id="96a0f-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="96a0f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="96a0f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96a0f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96a0f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a0f-132">Request</span></span>
<span data-ttu-id="96a0f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96a0f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96a0f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96a0f-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96a0f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96a0f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="96a0f-136">C#</span><span class="sxs-lookup"><span data-stu-id="96a0f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96a0f-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="96a0f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="96a0f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a0f-138">Response</span></span>
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
