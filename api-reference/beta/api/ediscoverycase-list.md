---
title: Listar ediscoveryCases
description: Recupere uma lista de ocorrências de descoberta eletrônica.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 4006e33bde696a8f92d1d77ff6a6cd8f55f13a54
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007957"
---
# <a name="list-ediscoverycases"></a><span data-ttu-id="506b7-103">Listar ediscoveryCases</span><span class="sxs-lookup"><span data-stu-id="506b7-103">List ediscoveryCases</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="506b7-104">Recupere uma lista de objetos [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="506b7-104">Retrieve a list of [ediscoveryCase](../resources/ediscoverycase.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="506b7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="506b7-105">Permissions</span></span>

<span data-ttu-id="506b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="506b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="506b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="506b7-108">Permission type</span></span>                        | <span data-ttu-id="506b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="506b7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="506b7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="506b7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="506b7-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="506b7-111">User.Read</span></span> |
| <span data-ttu-id="506b7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="506b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="506b7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="506b7-113">Not supported.</span></span> |
| <span data-ttu-id="506b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="506b7-114">Application</span></span>                            | <span data-ttu-id="506b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="506b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="506b7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="506b7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases
```

## <a name="optional-query-parameters"></a><span data-ttu-id="506b7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="506b7-117">Optional query parameters</span></span>

<span data-ttu-id="506b7-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="506b7-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="506b7-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="506b7-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="506b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="506b7-120">Request headers</span></span>

| <span data-ttu-id="506b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="506b7-121">Name</span></span>      |<span data-ttu-id="506b7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="506b7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="506b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="506b7-123">Authorization</span></span> | <span data-ttu-id="506b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="506b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="506b7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="506b7-126">Request body</span></span>

<span data-ttu-id="506b7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="506b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="506b7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="506b7-128">Response</span></span>

<span data-ttu-id="506b7-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [ediscoveryCase](../resources/ediscoverycase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="506b7-129">If successful, this method returns a `200 OK` response code and a collection of [ediscoveryCase](../resources/ediscoverycase.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="506b7-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="506b7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="506b7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="506b7-131">Request</span></span>

<span data-ttu-id="506b7-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="506b7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="506b7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="506b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoverycase"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```
# <a name="c"></a>[<span data-ttu-id="506b7-134">C#</span><span class="sxs-lookup"><span data-stu-id="506b7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="506b7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="506b7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="506b7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="506b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="506b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="506b7-137">Response</span></span>

<span data-ttu-id="506b7-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="506b7-138">The following is an example of the response.</span></span>

> <span data-ttu-id="506b7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="506b7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase",
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


