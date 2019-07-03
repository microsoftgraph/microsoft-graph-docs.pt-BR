---
title: Obter o ponto de extremidade
description: Recupere as propriedades e os relacionamentos de um objeto Endpoint específico.
localization_priority: Normal
ms.openlocfilehash: 78b1dd46e39fa25ecc77f257726d6884086c87a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441153"
---
# <a name="get-endpoint"></a><span data-ttu-id="d25a0-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="d25a0-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d25a0-104">Recupere as propriedades e os relacionamentos de um objeto [Endpoint](../resources/endpoint.md) específico.</span><span class="sxs-lookup"><span data-stu-id="d25a0-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d25a0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d25a0-105">Permissions</span></span>
<span data-ttu-id="d25a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d25a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d25a0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d25a0-108">Permission type</span></span>      | <span data-ttu-id="d25a0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d25a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d25a0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d25a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d25a0-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25a0-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d25a0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d25a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d25a0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d25a0-113">Not supported.</span></span>    |
|<span data-ttu-id="d25a0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d25a0-114">Application</span></span> | <span data-ttu-id="d25a0-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25a0-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d25a0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d25a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d25a0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d25a0-117">Optional query parameters</span></span>
<span data-ttu-id="d25a0-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d25a0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d25a0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d25a0-119">Request headers</span></span>
| <span data-ttu-id="d25a0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d25a0-120">Name</span></span>      |<span data-ttu-id="d25a0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d25a0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d25a0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d25a0-122">Authorization</span></span>  | <span data-ttu-id="d25a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d25a0-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d25a0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d25a0-125">Content-Type</span></span>   | <span data-ttu-id="d25a0-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="d25a0-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d25a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d25a0-127">Request body</span></span>
<span data-ttu-id="d25a0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d25a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d25a0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25a0-129">Response</span></span>

<span data-ttu-id="d25a0-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d25a0-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d25a0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d25a0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d25a0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d25a0-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d25a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d25a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d25a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="d25a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d25a0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d25a0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d25a0-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d25a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d25a0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25a0-137">Response</span></span>
<span data-ttu-id="d25a0-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d25a0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
