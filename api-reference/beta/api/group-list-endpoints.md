---
title: Listar pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 36e17cef09898dd65bf8fd3fa5af8c4dfdb95f13
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263144"
---
# <a name="list-endpoints"></a><span data-ttu-id="e7d60-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="e7d60-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d60-104">Recupere uma lista de objetos de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="e7d60-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7d60-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7d60-105">Permissions</span></span>
<span data-ttu-id="e7d60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d60-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7d60-108">Permission type</span></span>      | <span data-ttu-id="e7d60-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7d60-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7d60-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d60-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7d60-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d60-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7d60-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7d60-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7d60-113">Not supported.</span></span>    |
|<span data-ttu-id="e7d60-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d60-114">Application</span></span> | <span data-ttu-id="e7d60-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d60-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7d60-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d60-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7d60-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7d60-117">Optional query parameters</span></span>
<span data-ttu-id="e7d60-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d60-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7d60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d60-119">Request headers</span></span>
| <span data-ttu-id="e7d60-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e7d60-120">Name</span></span>      |<span data-ttu-id="e7d60-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d60-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7d60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d60-122">Authorization</span></span>  | <span data-ttu-id="e7d60-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d60-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e7d60-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7d60-125">Content-Type</span></span>   | <span data-ttu-id="e7d60-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="e7d60-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7d60-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d60-127">Request body</span></span>
<span data-ttu-id="e7d60-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7d60-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d60-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d60-129">Response</span></span>

<span data-ttu-id="e7d60-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d60-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7d60-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d60-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7d60-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d60-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="e7d60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d60-133">Response</span></span>
<span data-ttu-id="e7d60-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7d60-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7d60-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e7d60-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7d60-137">C#</span><span class="sxs-lookup"><span data-stu-id="e7d60-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_endpoints-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7d60-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7d60-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_endpoints-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e7d60-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e7d60-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_endpoints-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
