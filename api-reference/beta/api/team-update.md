---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dd247397c0445fca2969d75c85b46049a59d8ac0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076645"
---
# <a name="update-team"></a><span data-ttu-id="df3a6-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="df3a6-103">Update team</span></span>

<span data-ttu-id="df3a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df3a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df3a6-105">Atualize as propriedades da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="df3a6-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df3a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df3a6-106">Permissions</span></span>
<span data-ttu-id="df3a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df3a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="df3a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df3a6-109">Permission type</span></span>      | <span data-ttu-id="df3a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df3a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df3a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df3a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df3a6-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df3a6-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="df3a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df3a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df3a6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df3a6-114">Not supported.</span></span>    |
|<span data-ttu-id="df3a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df3a6-115">Application</span></span> | <span data-ttu-id="df3a6-116">TeamSettings. Edit. Group \*, TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="df3a6-116">TeamSettings.Edit.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="df3a6-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="df3a6-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="df3a6-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="df3a6-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="df3a6-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="df3a6-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="df3a6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df3a6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="df3a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df3a6-121">Request headers</span></span>
| <span data-ttu-id="df3a6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df3a6-122">Header</span></span>       | <span data-ttu-id="df3a6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="df3a6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df3a6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="df3a6-124">Authorization</span></span>  | <span data-ttu-id="df3a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df3a6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df3a6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df3a6-127">Content-Type</span></span>  | <span data-ttu-id="df3a6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="df3a6-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df3a6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df3a6-129">Request body</span></span>
<span data-ttu-id="df3a6-130">No corpo da solicitação, forneça uma representação JSON do objeto [Team](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="df3a6-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df3a6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="df3a6-131">Response</span></span>

<span data-ttu-id="df3a6-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df3a6-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df3a6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df3a6-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="df3a6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df3a6-134">Request</span></span>
<span data-ttu-id="df3a6-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df3a6-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df3a6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="df3a6-136">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="df3a6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df3a6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="df3a6-138">C#</span><span class="sxs-lookup"><span data-stu-id="df3a6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df3a6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df3a6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="df3a6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="df3a6-140">Response</span></span>
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


