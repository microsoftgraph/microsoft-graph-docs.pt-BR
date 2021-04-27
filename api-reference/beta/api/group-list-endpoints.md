---
title: Listar pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ea2517eeac7109d89563cb78989bc32c4bf7b5ba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041649"
---
# <a name="list-endpoints"></a><span data-ttu-id="5cd60-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="5cd60-103">List endpoints</span></span>

<span data-ttu-id="5cd60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cd60-105">Recupere uma lista de [objetos de ponto de](../resources/endpoint.md) extremidade.</span><span class="sxs-lookup"><span data-stu-id="5cd60-105">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cd60-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5cd60-106">Permissions</span></span>
<span data-ttu-id="5cd60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cd60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cd60-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cd60-109">Permission type</span></span>      | <span data-ttu-id="5cd60-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5cd60-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cd60-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cd60-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5cd60-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd60-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5cd60-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cd60-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cd60-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cd60-114">Not supported.</span></span>    |
|<span data-ttu-id="5cd60-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cd60-115">Application</span></span> | <span data-ttu-id="5cd60-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd60-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cd60-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cd60-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5cd60-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5cd60-118">Optional query parameters</span></span>
<span data-ttu-id="5cd60-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd60-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cd60-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd60-120">Request headers</span></span>
| <span data-ttu-id="5cd60-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5cd60-121">Name</span></span>      |<span data-ttu-id="5cd60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cd60-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5cd60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cd60-123">Authorization</span></span>  | <span data-ttu-id="5cd60-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cd60-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5cd60-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cd60-126">Content-Type</span></span>   | <span data-ttu-id="5cd60-127">Application/Json</span><span class="sxs-lookup"><span data-stu-id="5cd60-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cd60-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd60-128">Request body</span></span>
<span data-ttu-id="5cd60-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cd60-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cd60-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd60-130">Response</span></span>

<span data-ttu-id="5cd60-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd60-131">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5cd60-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cd60-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5cd60-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd60-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5cd60-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cd60-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="5cd60-135">C#</span><span class="sxs-lookup"><span data-stu-id="5cd60-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cd60-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cd60-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cd60-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cd60-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5cd60-138">Java</span><span class="sxs-lookup"><span data-stu-id="5cd60-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5cd60-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd60-139">Response</span></span>
<span data-ttu-id="5cd60-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd60-140">Here is an example of the response.</span></span>
><span data-ttu-id="5cd60-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5cd60-141">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
