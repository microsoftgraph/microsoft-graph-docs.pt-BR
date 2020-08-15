---
title: Atualizar equipe
description: Atualize as propriedades da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 02460579584a0b74cb884017e137c5537d5e4a53
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757255"
---
# <a name="update-team"></a><span data-ttu-id="1a7ad-103">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="1a7ad-103">Update team</span></span>

<span data-ttu-id="1a7ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a7ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a7ad-105">Atualize as propriedades da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a7ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a7ad-106">Permissions</span></span>
<span data-ttu-id="1a7ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a7ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a7ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a7ad-109">Permission type</span></span>      | <span data-ttu-id="1a7ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a7ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a7ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a7ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1a7ad-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a7ad-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1a7ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a7ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a7ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-114">Not supported.</span></span>    |
|<span data-ttu-id="1a7ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a7ad-115">Application</span></span> | <span data-ttu-id="1a7ad-116">TeamSettings. Edit. Group \*, TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1a7ad-116">TeamSettings.Edit.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1a7ad-117">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1a7ad-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="1a7ad-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1a7ad-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a7ad-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a7ad-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1a7ad-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7ad-121">Request headers</span></span>
| <span data-ttu-id="1a7ad-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a7ad-122">Header</span></span>       | <span data-ttu-id="1a7ad-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1a7ad-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a7ad-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a7ad-124">Authorization</span></span>  | <span data-ttu-id="1a7ad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1a7ad-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a7ad-127">Content-Type</span></span>  | <span data-ttu-id="1a7ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1a7ad-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a7ad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7ad-129">Request body</span></span>
<span data-ttu-id="1a7ad-130">No corpo da solicitação, forneça uma representação JSON do objeto [Team](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="1a7ad-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1a7ad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a7ad-131">Response</span></span>

<span data-ttu-id="1a7ad-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1a7ad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a7ad-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1a7ad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7ad-134">Request</span></span>
<span data-ttu-id="1a7ad-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a7ad-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a7ad-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a7ad-136">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1a7ad-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a7ad-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1a7ad-138">C#</span><span class="sxs-lookup"><span data-stu-id="1a7ad-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a7ad-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a7ad-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1a7ad-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a7ad-140">Response</span></span>
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
