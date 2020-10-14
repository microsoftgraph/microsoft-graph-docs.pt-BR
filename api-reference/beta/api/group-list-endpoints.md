---
title: Listar pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e7dcb0d269f1689a449840bbe2d805f78d19ec37
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457930"
---
# <a name="list-endpoints"></a><span data-ttu-id="83082-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="83082-103">List endpoints</span></span>

<span data-ttu-id="83082-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83082-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83082-105">Recupere uma lista de objetos de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="83082-105">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="83082-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83082-106">Permissions</span></span>
<span data-ttu-id="83082-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83082-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83082-109">Permission type</span></span>      | <span data-ttu-id="83082-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83082-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83082-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83082-111">Delegated (work or school account)</span></span> | <span data-ttu-id="83082-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83082-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83082-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83082-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83082-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83082-114">Not supported.</span></span>    |
|<span data-ttu-id="83082-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83082-115">Application</span></span> | <span data-ttu-id="83082-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83082-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83082-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83082-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83082-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83082-118">Optional query parameters</span></span>
<span data-ttu-id="83082-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83082-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83082-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83082-120">Request headers</span></span>
| <span data-ttu-id="83082-121">Nome</span><span class="sxs-lookup"><span data-stu-id="83082-121">Name</span></span>      |<span data-ttu-id="83082-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="83082-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83082-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83082-123">Authorization</span></span>  | <span data-ttu-id="83082-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83082-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="83082-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83082-126">Content-Type</span></span>   | <span data-ttu-id="83082-127">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="83082-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="83082-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83082-128">Request body</span></span>
<span data-ttu-id="83082-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83082-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83082-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="83082-130">Response</span></span>

<span data-ttu-id="83082-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83082-131">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83082-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83082-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="83082-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83082-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="83082-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="83082-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="83082-135">C#</span><span class="sxs-lookup"><span data-stu-id="83082-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83082-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83082-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83082-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83082-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="83082-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="83082-138">Response</span></span>
<span data-ttu-id="83082-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83082-139">Here is an example of the response.</span></span>
><span data-ttu-id="83082-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83082-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
