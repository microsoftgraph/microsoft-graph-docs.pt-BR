---
title: Obter canal
description: Recuperar as propriedades e os relacionamentos de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8690a832484b607e3dcb788232b599952e49fdd0
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633409"
---
# <a name="get-channel"></a><span data-ttu-id="8dc70-103">Obter canal</span><span class="sxs-lookup"><span data-stu-id="8dc70-103">Get channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dc70-104">Recuperar as propriedades e os relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8dc70-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8dc70-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8dc70-105">Permissions</span></span>

<span data-ttu-id="8dc70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dc70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dc70-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dc70-108">Permission type</span></span>      | <span data-ttu-id="8dc70-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dc70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dc70-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dc70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8dc70-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc70-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8dc70-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dc70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dc70-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dc70-113">Not supported.</span></span>    |
|<span data-ttu-id="8dc70-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dc70-114">Application</span></span> | <span data-ttu-id="8dc70-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc70-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8dc70-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8dc70-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8dc70-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8dc70-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8dc70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc70-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="8dc70-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8dc70-119">Optional query parameters</span></span>

<span data-ttu-id="8dc70-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8dc70-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dc70-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc70-121">Request headers</span></span>

| <span data-ttu-id="8dc70-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8dc70-122">Header</span></span>       | <span data-ttu-id="8dc70-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8dc70-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8dc70-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dc70-124">Authorization</span></span>  | <span data-ttu-id="8dc70-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dc70-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8dc70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc70-127">Request body</span></span>

<span data-ttu-id="8dc70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8dc70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dc70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dc70-129">Response</span></span>

<span data-ttu-id="8dc70-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dc70-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dc70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dc70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dc70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc70-132">Request</span></span>

<span data-ttu-id="8dc70-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dc70-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8dc70-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc70-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="8dc70-135">C#</span><span class="sxs-lookup"><span data-stu-id="8dc70-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8dc70-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dc70-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8dc70-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8dc70-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8dc70-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dc70-138">Response</span></span>

<span data-ttu-id="8dc70-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dc70-139">Here is an example of the response.</span></span>

><span data-ttu-id="8dc70-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dc70-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value",
    "membershipType": "membership-type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
