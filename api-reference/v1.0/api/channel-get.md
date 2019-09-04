---
title: Obter canal
description: Recuperar as propriedades e os relacionamentos de um canal.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa95725a6edc1fb3d8cee0502e453de355f38615
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726477"
---
# <a name="get-channel"></a><span data-ttu-id="d69a3-103">Obter canal</span><span class="sxs-lookup"><span data-stu-id="d69a3-103">Get channel</span></span>



<span data-ttu-id="d69a3-104">Recuperar as propriedades e os relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="d69a3-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d69a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d69a3-105">Permissions</span></span>
<span data-ttu-id="d69a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d69a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d69a3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d69a3-108">Permission type</span></span>      | <span data-ttu-id="d69a3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d69a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d69a3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d69a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d69a3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d69a3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d69a3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d69a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d69a3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d69a3-113">Not supported.</span></span>    |
|<span data-ttu-id="d69a3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d69a3-114">Application</span></span> | <span data-ttu-id="d69a3-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d69a3-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="d69a3-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d69a3-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d69a3-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d69a3-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d69a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d69a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="d69a3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d69a3-119">Optional query parameters</span></span>

<span data-ttu-id="d69a3-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d69a3-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d69a3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d69a3-121">Request headers</span></span>
| <span data-ttu-id="d69a3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d69a3-122">Header</span></span>       | <span data-ttu-id="d69a3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d69a3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d69a3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d69a3-124">Authorization</span></span>  | <span data-ttu-id="d69a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d69a3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d69a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d69a3-127">Request body</span></span>
<span data-ttu-id="d69a3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d69a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d69a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d69a3-129">Response</span></span>

<span data-ttu-id="d69a3-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d69a3-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d69a3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d69a3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d69a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d69a3-132">Request</span></span>
<span data-ttu-id="d69a3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d69a3-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d69a3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d69a3-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d69a3-135">C#</span><span class="sxs-lookup"><span data-stu-id="d69a3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d69a3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d69a3-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d69a3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d69a3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d69a3-138">Java</span><span class="sxs-lookup"><span data-stu-id="d69a3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d69a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d69a3-139">Response</span></span>
<span data-ttu-id="d69a3-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d69a3-140">Here is an example of the response.</span></span> 

><span data-ttu-id="d69a3-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d69a3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
