---
title: Listar sourceCollections
description: Obter a lista de recursos sourceCollections de um objeto case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2902b13af183a72a20a4322ff9d78357d150e4a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776589"
---
# <a name="list-sourcecollections"></a><span data-ttu-id="0c8a3-103">Listar sourceCollections</span><span class="sxs-lookup"><span data-stu-id="0c8a3-103">List sourceCollections</span></span>

<span data-ttu-id="0c8a3-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0c8a3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c8a3-105">Obter a lista [de sourceCollections](../resources/ediscovery-sourcecollection.md) de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="0c8a3-105">Get the list of [sourceCollections](../resources/ediscovery-sourcecollection.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c8a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c8a3-106">Permissions</span></span>

<span data-ttu-id="0c8a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c8a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c8a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c8a3-109">Permission type</span></span>|<span data-ttu-id="0c8a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c8a3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c8a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c8a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c8a3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8a3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0c8a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c8a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c8a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-114">Not supported.</span></span>|
|<span data-ttu-id="0c8a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c8a3-115">Application</span></span>|<span data-ttu-id="0c8a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c8a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c8a3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c8a3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0c8a3-118">Optional query parameters</span></span>

<span data-ttu-id="0c8a3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0c8a3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0c8a3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c8a3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c8a3-121">Request headers</span></span>

|<span data-ttu-id="0c8a3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0c8a3-122">Name</span></span>|<span data-ttu-id="0c8a3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c8a3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c8a3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c8a3-124">Authorization</span></span>|<span data-ttu-id="0c8a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c8a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c8a3-127">Request body</span></span>

<span data-ttu-id="0c8a3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c8a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c8a3-129">Response</span></span>

<span data-ttu-id="0c8a3-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c8a3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0c8a3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c8a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c8a3-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0c8a3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c8a3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections
```
# <a name="c"></a>[<span data-ttu-id="0c8a3-134">C#</span><span class="sxs-lookup"><span data-stu-id="0c8a3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c8a3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c8a3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c8a3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c8a3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c8a3-137">Java</span><span class="sxs-lookup"><span data-stu-id="0c8a3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c8a3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c8a3-138">Response</span></span>

<span data-ttu-id="0c8a3-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c8a3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.sourceCollection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/sourceCollections",
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2020-12-31T18:54:28.80694Z",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "contentQuery": "subject:'Quarterly Financials'",
            "tenantSources": "none",
            "id": "fe5ef84e9c8c45819c056f6eb261718e",
            "displayName": "Quarterly Financials",
            "createdDateTime": "2020-12-11T22:56:14.2329133Z"
        }
    ]
}
```
