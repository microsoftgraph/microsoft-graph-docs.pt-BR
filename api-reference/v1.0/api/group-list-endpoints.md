---
title: Listar pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f3bd3ae6d49e6f101872f5c38a0b0e85395c7f9a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459708"
---
# <a name="list-endpoints"></a><span data-ttu-id="6e0b7-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="6e0b7-103">List endpoints</span></span>

<span data-ttu-id="6e0b7-104">Recupere uma lista de objetos de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="6e0b7-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e0b7-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e0b7-105">Permissions</span></span>
<span data-ttu-id="6e0b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e0b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e0b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e0b7-108">Permission type</span></span>      | <span data-ttu-id="6e0b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e0b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e0b7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e0b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e0b7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0b7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e0b7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e0b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e0b7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-113">Not supported.</span></span>    |
|<span data-ttu-id="6e0b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e0b7-114">Application</span></span> | <span data-ttu-id="6e0b7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0b7-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e0b7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e0b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e0b7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e0b7-117">Optional query parameters</span></span>
<span data-ttu-id="6e0b7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e0b7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e0b7-119">Request headers</span></span>
| <span data-ttu-id="6e0b7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6e0b7-120">Name</span></span>      |<span data-ttu-id="6e0b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e0b7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e0b7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e0b7-122">Authorization</span></span>  | <span data-ttu-id="6e0b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6e0b7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e0b7-125">Content-Type</span></span>   | <span data-ttu-id="6e0b7-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="6e0b7-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e0b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e0b7-127">Request body</span></span>
<span data-ttu-id="6e0b7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e0b7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e0b7-129">Response</span></span>

<span data-ttu-id="6e0b7-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-130">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e0b7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e0b7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e0b7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e0b7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6e0b7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e0b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="6e0b7-134">C#</span><span class="sxs-lookup"><span data-stu-id="6e0b7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e0b7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e0b7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e0b7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e0b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e0b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e0b7-137">Response</span></span>
<span data-ttu-id="6e0b7-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-138">Here is an example of the response.</span></span>
><span data-ttu-id="6e0b7-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e0b7-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
