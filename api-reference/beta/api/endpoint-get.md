---
title: Obter o ponto de extremidade
description: Recupere as propriedades e os relacionamentos de um objeto Endpoint específico.
localization_priority: Normal
ms.openlocfilehash: 9c43c965fe5210df035f1b7a6bb6b553c4f40540
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587168"
---
# <a name="get-endpoint"></a><span data-ttu-id="067c5-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="067c5-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="067c5-104">Recupere as propriedades e os relacionamentos de um objeto [Endpoint](../resources/endpoint.md) específico.</span><span class="sxs-lookup"><span data-stu-id="067c5-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="067c5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="067c5-105">Permissions</span></span>
<span data-ttu-id="067c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="067c5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="067c5-108">Permission type</span></span>      | <span data-ttu-id="067c5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="067c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="067c5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="067c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="067c5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="067c5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="067c5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="067c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="067c5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="067c5-113">Not supported.</span></span>    |
|<span data-ttu-id="067c5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="067c5-114">Application</span></span> | <span data-ttu-id="067c5-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="067c5-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="067c5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="067c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="067c5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="067c5-117">Optional query parameters</span></span>
<span data-ttu-id="067c5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="067c5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="067c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="067c5-119">Request headers</span></span>
| <span data-ttu-id="067c5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="067c5-120">Name</span></span>      |<span data-ttu-id="067c5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="067c5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="067c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="067c5-122">Authorization</span></span>  | <span data-ttu-id="067c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="067c5-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="067c5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="067c5-125">Content-Type</span></span>   | <span data-ttu-id="067c5-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="067c5-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="067c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="067c5-127">Request body</span></span>
<span data-ttu-id="067c5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="067c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="067c5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="067c5-129">Response</span></span>

<span data-ttu-id="067c5-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="067c5-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="067c5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="067c5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="067c5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="067c5-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="067c5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="067c5-133">Response</span></span>
<span data-ttu-id="067c5-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="067c5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="067c5-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="067c5-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="067c5-137">Basic</span><span class="sxs-lookup"><span data-stu-id="067c5-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_endpoint-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="067c5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="067c5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_endpoint-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
