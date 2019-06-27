---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a2d127070e35f5c09e4b59dcf1e9ae4b4e858267
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271754"
---
# <a name="update-team"></a><span data-ttu-id="dc850-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="dc850-103">Update team</span></span>



<span data-ttu-id="dc850-104">Atualize as propriedades da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="dc850-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc850-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc850-105">Permissions</span></span>
<span data-ttu-id="dc850-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dc850-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc850-108">Permission type</span></span>      | <span data-ttu-id="dc850-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc850-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc850-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc850-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc850-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc850-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc850-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc850-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc850-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc850-113">Not supported.</span></span>    |
|<span data-ttu-id="dc850-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc850-114">Application</span></span> | <span data-ttu-id="dc850-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc850-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="dc850-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="dc850-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dc850-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="dc850-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dc850-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc850-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc850-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc850-119">Request headers</span></span>
| <span data-ttu-id="dc850-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc850-120">Header</span></span>       | <span data-ttu-id="dc850-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc850-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc850-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc850-122">Authorization</span></span>  | <span data-ttu-id="dc850-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc850-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc850-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc850-125">Content-Type</span></span>  | <span data-ttu-id="dc850-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc850-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc850-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc850-127">Request body</span></span>
<span data-ttu-id="dc850-128">No corpo da solicitação, forneça uma representação JSON do objeto [Team](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="dc850-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dc850-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc850-129">Response</span></span>

<span data-ttu-id="dc850-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc850-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc850-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc850-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dc850-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc850-132">Request</span></span>
<span data-ttu-id="dc850-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc850-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}
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
  }
}
```
#### <a name="response"></a><span data-ttu-id="dc850-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc850-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dc850-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dc850-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dc850-136">C#</span><span class="sxs-lookup"><span data-stu-id="dc850-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_team-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc850-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc850-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_team-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dc850-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dc850-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_team-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/team-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/team-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/team-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
