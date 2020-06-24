---
title: Obter equipe
description: Recupere as propriedades e relações da equipe especificada.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc9a45e22022b6f95ab0e7dde4187bfe105af093
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845796"
---
# <a name="get-team"></a><span data-ttu-id="e7482-103">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="e7482-103">Get team</span></span>

<span data-ttu-id="e7482-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7482-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e7482-105">Recupere as propriedades e relações da [equipe](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="e7482-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7482-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7482-106">Permissions</span></span>
<span data-ttu-id="e7482-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e7482-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e7482-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7482-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7482-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7482-109">Permission type</span></span>      | <span data-ttu-id="e7482-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7482-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7482-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7482-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7482-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7482-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7482-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7482-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7482-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7482-114">Not supported.</span></span>    |
|<span data-ttu-id="e7482-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7482-115">Application</span></span> | <span data-ttu-id="e7482-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7482-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="e7482-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e7482-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e7482-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e7482-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7482-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7482-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7482-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7482-120">Optional query parameters</span></span>
<span data-ttu-id="e7482-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7482-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7482-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7482-122">Request headers</span></span>
| <span data-ttu-id="e7482-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7482-123">Header</span></span>       | <span data-ttu-id="e7482-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e7482-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7482-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7482-125">Authorization</span></span>  | <span data-ttu-id="e7482-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e7482-126">Bearer {token}.</span></span> <span data-ttu-id="e7482-127">Required.</span><span class="sxs-lookup"><span data-stu-id="e7482-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7482-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7482-128">Request body</span></span>
<span data-ttu-id="e7482-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7482-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7482-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7482-130">Response</span></span>

<span data-ttu-id="e7482-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7482-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7482-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7482-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e7482-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7482-133">Request</span></span>
<span data-ttu-id="e7482-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7482-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7482-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7482-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}
```
# <a name="c"></a>[<span data-ttu-id="e7482-136">C#</span><span class="sxs-lookup"><span data-stu-id="e7482-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7482-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7482-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7482-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7482-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7482-139">Java</span><span class="sxs-lookup"><span data-stu-id="e7482-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e7482-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7482-140">Response</span></span>
<span data-ttu-id="e7482-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7482-141">The following is an example of the response.</span></span> 

><span data-ttu-id="e7482-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="e7482-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7482-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e7482-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived": false,
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  },
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
