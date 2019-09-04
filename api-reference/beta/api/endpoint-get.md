---
title: Obter o ponto de extremidade
description: Recupere as propriedades e os relacionamentos de um objeto Endpoint específico.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: f7ca844d59afe133781c0b3bce7d1577c79efb1e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720701"
---
# <a name="get-endpoint"></a><span data-ttu-id="a2b2c-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="a2b2c-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2b2c-104">Recupere as propriedades e os relacionamentos de um objeto [Endpoint](../resources/endpoint.md) específico.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2b2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2b2c-105">Permissions</span></span>
<span data-ttu-id="a2b2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2b2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a2b2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2b2c-108">Permission type</span></span>      | <span data-ttu-id="a2b2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2b2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2b2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2b2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2b2c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b2c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2b2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2b2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2b2c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-113">Not supported.</span></span>    |
|<span data-ttu-id="a2b2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2b2c-114">Application</span></span> | <span data-ttu-id="a2b2c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b2c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2b2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2b2c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2b2c-117">Optional query parameters</span></span>
<span data-ttu-id="a2b2c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2b2c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b2c-119">Request headers</span></span>
| <span data-ttu-id="a2b2c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a2b2c-120">Name</span></span>      |<span data-ttu-id="a2b2c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2b2c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2b2c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2b2c-122">Authorization</span></span>  | <span data-ttu-id="a2b2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a2b2c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2b2c-125">Content-Type</span></span>   | <span data-ttu-id="a2b2c-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="a2b2c-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2b2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b2c-127">Request body</span></span>
<span data-ttu-id="a2b2c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2b2c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b2c-129">Response</span></span>

<span data-ttu-id="a2b2c-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2b2c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2b2c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2b2c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b2c-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a2b2c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b2c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2b2c-134">C#</span><span class="sxs-lookup"><span data-stu-id="a2b2c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2b2c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2b2c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2b2c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a2b2c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a2b2c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b2c-137">Response</span></span>
<span data-ttu-id="a2b2c-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2b2c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
