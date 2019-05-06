---
title: Listar pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d1a3691fb704fec5e10304bc6a11539e8984c909
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593061"
---
# <a name="list-endpoints"></a><span data-ttu-id="9b859-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="9b859-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b859-104">Recupere uma lista de objetos de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="9b859-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b859-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b859-105">Permissions</span></span>
<span data-ttu-id="9b859-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b859-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b859-108">Permission type</span></span>      | <span data-ttu-id="9b859-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b859-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b859-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b859-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b859-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b859-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b859-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b859-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b859-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b859-113">Not supported.</span></span>    |
|<span data-ttu-id="9b859-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b859-114">Application</span></span> | <span data-ttu-id="9b859-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b859-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b859-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b859-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9b859-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b859-117">Optional query parameters</span></span>
<span data-ttu-id="9b859-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b859-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b859-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b859-119">Request headers</span></span>
| <span data-ttu-id="9b859-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9b859-120">Name</span></span>      |<span data-ttu-id="9b859-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b859-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b859-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b859-122">Authorization</span></span>  | <span data-ttu-id="9b859-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b859-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9b859-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b859-125">Content-Type</span></span>   | <span data-ttu-id="9b859-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="9b859-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b859-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b859-127">Request body</span></span>
<span data-ttu-id="9b859-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b859-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b859-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b859-129">Response</span></span>

<span data-ttu-id="9b859-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b859-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b859-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b859-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b859-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b859-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="9b859-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b859-133">Response</span></span>
<span data-ttu-id="9b859-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b859-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b859-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9b859-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b859-137">Basic</span><span class="sxs-lookup"><span data-stu-id="9b859-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_endpoints-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b859-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b859-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_endpoints-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
