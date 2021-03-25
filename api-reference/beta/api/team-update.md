---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1d001949ac60b8d3c6335bf4a6e79cba5488c072
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202258"
---
# <a name="update-team"></a><span data-ttu-id="d9194-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="d9194-103">Update team</span></span>

<span data-ttu-id="d9194-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9194-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9194-105">Atualize as propriedades da equipe [especificada](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d9194-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9194-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9194-106">Permissions</span></span>
<span data-ttu-id="d9194-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9194-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9194-109">Permission type</span></span>      | <span data-ttu-id="d9194-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9194-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9194-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9194-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9194-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9194-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d9194-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9194-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9194-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9194-114">Not supported.</span></span>    |
|<span data-ttu-id="d9194-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9194-115">Application</span></span> | <span data-ttu-id="d9194-116">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9194-116">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d9194-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d9194-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d9194-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d9194-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d9194-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d9194-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9194-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9194-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}
```
## <a name="request-headers"></a><span data-ttu-id="d9194-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9194-121">Request headers</span></span>
| <span data-ttu-id="d9194-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9194-122">Header</span></span>       | <span data-ttu-id="d9194-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d9194-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9194-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9194-124">Authorization</span></span>  | <span data-ttu-id="d9194-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9194-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d9194-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9194-127">Content-Type</span></span>  | <span data-ttu-id="d9194-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d9194-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9194-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9194-129">Request body</span></span>
<span data-ttu-id="d9194-130">No corpo da solicitação, fornece uma representação JSON do [objeto team.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="d9194-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9194-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9194-131">Response</span></span>

<span data-ttu-id="d9194-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9194-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9194-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9194-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d9194-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9194-134">Request</span></span>
<span data-ttu-id="d9194-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9194-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9194-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9194-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
 "isMembershipLimitedToOwners": true,
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
# <a name="javascript"></a>[<span data-ttu-id="d9194-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9194-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d9194-138">C#</span><span class="sxs-lookup"><span data-stu-id="d9194-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9194-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9194-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9194-140">Java</span><span class="sxs-lookup"><span data-stu-id="d9194-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d9194-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9194-141">Response</span></span>
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


