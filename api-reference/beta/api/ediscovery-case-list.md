---
title: Listar casos
description: Recupere uma lista de casos de Descoberta e.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: eae0e826451383eb4e3bbd9b2c8089709baf509e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044757"
---
# <a name="list-cases"></a><span data-ttu-id="1f82b-103">Listar casos</span><span class="sxs-lookup"><span data-stu-id="1f82b-103">List cases</span></span>

<span data-ttu-id="1f82b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1f82b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f82b-105">Recupere uma lista de [objetos case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="1f82b-105">Retrieve a list of [case](../resources/ediscovery-case.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f82b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f82b-106">Permissions</span></span>

<span data-ttu-id="1f82b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f82b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f82b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f82b-109">Permission type</span></span>|<span data-ttu-id="1f82b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f82b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f82b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f82b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f82b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f82b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1f82b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f82b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f82b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f82b-114">Not supported.</span></span>|
|<span data-ttu-id="1f82b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f82b-115">Application</span></span>|<span data-ttu-id="1f82b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f82b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f82b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f82b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f82b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f82b-118">Optional query parameters</span></span>

<span data-ttu-id="1f82b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f82b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1f82b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f82b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f82b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f82b-121">Request headers</span></span>

| <span data-ttu-id="1f82b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1f82b-122">Name</span></span>      |<span data-ttu-id="1f82b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f82b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f82b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f82b-124">Authorization</span></span> | <span data-ttu-id="1f82b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f82b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f82b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f82b-127">Request body</span></span>

<span data-ttu-id="1f82b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f82b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f82b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f82b-129">Response</span></span>

<span data-ttu-id="1f82b-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f82b-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f82b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1f82b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f82b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f82b-132">Request</span></span>

<span data-ttu-id="1f82b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f82b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f82b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f82b-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "list_case"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```

# <a name="c"></a>[<span data-ttu-id="1f82b-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f82b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f82b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f82b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f82b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f82b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f82b-138">Java</span><span class="sxs-lookup"><span data-stu-id="1f82b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1f82b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f82b-139">Response</span></span>

<span data-ttu-id="1f82b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f82b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1f82b-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f82b-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "odata.nextLink":"https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skipToken=159dc1d7-f84f-439e-9d57-4a4d3af0abe5",
    "value": [
        {
            "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
            "displayName": "My Case 1",
            "description": "",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-02-20T22:42:28.5505500Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
            "status": "active",
            "closedBy": null,
            "closedDateTime": null,
            "externalId": ""
        },
        {
            "id": "b956a1b5-6b74-47db-af83-97d1fdad4ddc",
            "displayName": "My Case 2",
            "description": "",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-02-18T22:42:28.5505500Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-02-18T22:42:28.5505500Z",
            "status": "active",
            "closedBy": null,
            "closedDateTime": null,
            "externalId": ""
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List cases",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
