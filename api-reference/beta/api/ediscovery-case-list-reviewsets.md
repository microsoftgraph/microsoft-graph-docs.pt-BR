---
title: Listar reviewSets
description: Obter os recursos reviewSet de um objeto case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1ef80d6801cad9405d4089c548ef8ad93e0bd794
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776645"
---
# <a name="list-reviewsets"></a><span data-ttu-id="88177-103">Listar reviewSets</span><span class="sxs-lookup"><span data-stu-id="88177-103">List reviewSets</span></span>

<span data-ttu-id="88177-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="88177-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88177-105">Obter a lista de [reviewSets](../resources/ediscovery-reviewset.md) de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="88177-105">Get the list of [reviewSets](../resources/ediscovery-reviewset.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88177-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88177-106">Permissions</span></span>

<span data-ttu-id="88177-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88177-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88177-109">Permission type</span></span>|<span data-ttu-id="88177-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88177-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88177-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88177-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88177-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88177-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="88177-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88177-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88177-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88177-114">Not supported.</span></span>|
|<span data-ttu-id="88177-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88177-115">Application</span></span>|<span data-ttu-id="88177-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88177-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88177-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88177-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/reviewSets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88177-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88177-118">Optional query parameters</span></span>

<span data-ttu-id="88177-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88177-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="88177-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="88177-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="88177-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88177-121">Request headers</span></span>

|<span data-ttu-id="88177-122">Nome</span><span class="sxs-lookup"><span data-stu-id="88177-122">Name</span></span>|<span data-ttu-id="88177-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="88177-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88177-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="88177-124">Authorization</span></span>|<span data-ttu-id="88177-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88177-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88177-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88177-127">Request body</span></span>

<span data-ttu-id="88177-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88177-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88177-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="88177-129">Response</span></span>

<span data-ttu-id="88177-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88177-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88177-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="88177-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88177-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88177-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88177-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="88177-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/reviewSets
```
# <a name="c"></a>[<span data-ttu-id="88177-134">C#</span><span class="sxs-lookup"><span data-stu-id="88177-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88177-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88177-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88177-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88177-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88177-137">Java</span><span class="sxs-lookup"><span data-stu-id="88177-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88177-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="88177-138">Response</span></span>

<span data-ttu-id="88177-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="88177-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.reviewSet)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skiptoken=<encodedPageToken>",
    "value": [
        {
            "id": "f6a91542-4ce7-4712-b275-c29545dd8507",
            "displayName": "My Reviewset 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T11:58:27.1408174Z"
        },
        {
            "id": "0d78ec4a-aa91-41ea-8da8-d68b030c168f",
            "displayName": "My Reviewset 2",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T12:03:32.2038960Z"
        }
    ]
}
```
