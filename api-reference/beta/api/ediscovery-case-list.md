---
title: Listar casos
description: Recupere uma lista de casos de Descoberta e.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f2165f0149bc3389820907341773f78d1840ef26
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776568"
---
# <a name="list-cases"></a><span data-ttu-id="8aafe-103">Listar casos</span><span class="sxs-lookup"><span data-stu-id="8aafe-103">List cases</span></span>

<span data-ttu-id="8aafe-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8aafe-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aafe-105">Recupere uma lista de [objetos case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="8aafe-105">Retrieve a list of [case](../resources/ediscovery-case.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aafe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8aafe-106">Permissions</span></span>

<span data-ttu-id="8aafe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aafe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aafe-109">Permission type</span></span>|<span data-ttu-id="8aafe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8aafe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aafe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aafe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8aafe-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aafe-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8aafe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aafe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aafe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aafe-114">Not supported.</span></span>|
|<span data-ttu-id="8aafe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aafe-115">Application</span></span>|<span data-ttu-id="8aafe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aafe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aafe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aafe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8aafe-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8aafe-118">Optional query parameters</span></span>

<span data-ttu-id="8aafe-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8aafe-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8aafe-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8aafe-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aafe-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aafe-121">Request headers</span></span>

| <span data-ttu-id="8aafe-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8aafe-122">Name</span></span>      |<span data-ttu-id="8aafe-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aafe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8aafe-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aafe-124">Authorization</span></span> | <span data-ttu-id="8aafe-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aafe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aafe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aafe-127">Request body</span></span>

<span data-ttu-id="8aafe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8aafe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aafe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aafe-129">Response</span></span>

<span data-ttu-id="8aafe-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aafe-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aafe-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8aafe-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aafe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aafe-132">Request</span></span>

<span data-ttu-id="8aafe-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aafe-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8aafe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aafe-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "list_case"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```

# <a name="c"></a>[<span data-ttu-id="8aafe-135">C#</span><span class="sxs-lookup"><span data-stu-id="8aafe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8aafe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8aafe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8aafe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aafe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8aafe-138">Java</span><span class="sxs-lookup"><span data-stu-id="8aafe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8aafe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aafe-139">Response</span></span>

<span data-ttu-id="8aafe-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8aafe-140">The following is an example of the response.</span></span>

> <span data-ttu-id="8aafe-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aafe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
