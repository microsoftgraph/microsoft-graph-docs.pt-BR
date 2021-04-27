---
title: Obter o ponto de extremidade
description: Recupere as propriedades e as relações de um objeto de ponto de extremidade específico.
localization_priority: Normal
doc_type: apiPageType
ms.prod: groups
author: yyuank
ms.openlocfilehash: 8b5cc003787b9a389842389d3aabd7c75726c8f5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042643"
---
# <a name="get-endpoint"></a><span data-ttu-id="2334d-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="2334d-103">Get endpoint</span></span>

<span data-ttu-id="2334d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2334d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2334d-105">Recupere as propriedades e as relações de um objeto [de ponto de](../resources/endpoint.md) extremidade específico.</span><span class="sxs-lookup"><span data-stu-id="2334d-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2334d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2334d-106">Permissions</span></span>
<span data-ttu-id="2334d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2334d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2334d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2334d-109">Permission type</span></span>      | <span data-ttu-id="2334d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2334d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2334d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2334d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2334d-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2334d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2334d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2334d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2334d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2334d-114">Not supported.</span></span>    |
|<span data-ttu-id="2334d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2334d-115">Application</span></span> | <span data-ttu-id="2334d-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2334d-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2334d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2334d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2334d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2334d-118">Optional query parameters</span></span>
<span data-ttu-id="2334d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2334d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2334d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2334d-120">Request headers</span></span>
| <span data-ttu-id="2334d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2334d-121">Name</span></span>      |<span data-ttu-id="2334d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2334d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2334d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2334d-123">Authorization</span></span>  | <span data-ttu-id="2334d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2334d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2334d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2334d-126">Request body</span></span>
<span data-ttu-id="2334d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2334d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2334d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2334d-128">Response</span></span>

<span data-ttu-id="2334d-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2334d-129">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2334d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2334d-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="2334d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2334d-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2334d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2334d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="2334d-133">C#</span><span class="sxs-lookup"><span data-stu-id="2334d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2334d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2334d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2334d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2334d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2334d-136">Java</span><span class="sxs-lookup"><span data-stu-id="2334d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2334d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2334d-137">Response</span></span>
<span data-ttu-id="2334d-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2334d-138">Here is an example of the response.</span></span>
><span data-ttu-id="2334d-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2334d-139">Note: The response object shown here might be shortened for readability.</span></span>
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
