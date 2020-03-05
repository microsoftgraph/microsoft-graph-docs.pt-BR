---
title: Obter o ponto de extremidade
description: Recupere as propriedades e os relacionamentos de um objeto Endpoint específico.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 15ccf9b6a250cf75d613826899a30a0c8e20b420
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423487"
---
# <a name="get-endpoint"></a><span data-ttu-id="dd39f-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="dd39f-103">Get endpoint</span></span>

<span data-ttu-id="dd39f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd39f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd39f-105">Recupere as propriedades e os relacionamentos de um objeto [Endpoint](../resources/endpoint.md) específico.</span><span class="sxs-lookup"><span data-stu-id="dd39f-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd39f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd39f-106">Permissions</span></span>
<span data-ttu-id="dd39f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd39f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd39f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd39f-109">Permission type</span></span>      | <span data-ttu-id="dd39f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd39f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd39f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd39f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd39f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd39f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd39f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd39f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd39f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd39f-114">Not supported.</span></span>    |
|<span data-ttu-id="dd39f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd39f-115">Application</span></span> | <span data-ttu-id="dd39f-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd39f-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd39f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd39f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd39f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dd39f-118">Optional query parameters</span></span>
<span data-ttu-id="dd39f-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd39f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd39f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd39f-120">Request headers</span></span>
| <span data-ttu-id="dd39f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dd39f-121">Name</span></span>      |<span data-ttu-id="dd39f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd39f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd39f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd39f-123">Authorization</span></span>  | <span data-ttu-id="dd39f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd39f-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="dd39f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd39f-126">Content-Type</span></span>   | <span data-ttu-id="dd39f-127">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="dd39f-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd39f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd39f-128">Request body</span></span>
<span data-ttu-id="dd39f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd39f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd39f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd39f-130">Response</span></span>

<span data-ttu-id="dd39f-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd39f-131">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd39f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd39f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd39f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd39f-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dd39f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd39f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="dd39f-135">C#</span><span class="sxs-lookup"><span data-stu-id="dd39f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd39f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd39f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd39f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd39f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd39f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd39f-138">Response</span></span>
<span data-ttu-id="dd39f-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd39f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
