---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ec14407ba58a9e27692b9354ec689efacc3eff5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982428"
---
# <a name="update-team"></a><span data-ttu-id="cc090-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="cc090-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc090-104">Atualize as propriedades da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="cc090-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc090-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc090-105">Permissions</span></span>
<span data-ttu-id="cc090-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cc090-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc090-108">Permission type</span></span>      | <span data-ttu-id="cc090-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc090-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc090-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc090-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc090-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc090-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc090-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc090-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc090-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc090-113">Not supported.</span></span>    |
|<span data-ttu-id="cc090-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc090-114">Application</span></span> | <span data-ttu-id="cc090-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc090-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="cc090-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="cc090-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cc090-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="cc090-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc090-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc090-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cc090-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc090-119">Request headers</span></span>
| <span data-ttu-id="cc090-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc090-120">Header</span></span>       | <span data-ttu-id="cc090-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc090-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc090-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc090-122">Authorization</span></span>  | <span data-ttu-id="cc090-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc090-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc090-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc090-125">Content-Type</span></span>  | <span data-ttu-id="cc090-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc090-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc090-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc090-127">Request body</span></span>
<span data-ttu-id="cc090-128">No corpo da solicitação, forneça uma representação JSON do objeto [Team](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="cc090-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc090-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc090-129">Response</span></span>

<span data-ttu-id="cc090-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cc090-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cc090-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc090-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc090-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc090-132">Request</span></span>
<span data-ttu-id="cc090-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc090-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc090-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc090-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc090-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc090-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="cc090-136">C#</span><span class="sxs-lookup"><span data-stu-id="cc090-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc090-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cc090-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc090-138">Java</span><span class="sxs-lookup"><span data-stu-id="cc090-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cc090-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc090-139">Response</span></span>
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
