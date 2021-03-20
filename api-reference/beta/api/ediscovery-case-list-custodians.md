---
title: Listar custodiantes
description: Obter uma lista dos objetos custodiantes e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e106d3a861c556b4800cec6df7bf2cd1df5a55a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946394"
---
# <a name="list-custodians"></a><span data-ttu-id="bab89-103">Listar custodiantes</span><span class="sxs-lookup"><span data-stu-id="bab89-103">List custodians</span></span>

<span data-ttu-id="bab89-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bab89-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab89-105">Obter uma lista dos [objetos custodiantes](../resources/ediscovery-custodian.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="bab89-105">Get a list of the [custodian](../resources/ediscovery-custodian.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="bab89-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bab89-106">Permissions</span></span>

<span data-ttu-id="bab89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bab89-109">Permission type</span></span>|<span data-ttu-id="bab89-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bab89-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bab89-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bab89-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bab89-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab89-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bab89-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bab89-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bab89-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bab89-114">Not supported.</span></span>|
|<span data-ttu-id="bab89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bab89-115">Application</span></span>|<span data-ttu-id="bab89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bab89-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bab89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bab89-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bab89-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bab89-118">Optional query parameters</span></span>

<span data-ttu-id="bab89-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bab89-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bab89-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bab89-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab89-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bab89-121">Request headers</span></span>

|<span data-ttu-id="bab89-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bab89-122">Name</span></span>|<span data-ttu-id="bab89-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab89-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bab89-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bab89-124">Authorization</span></span>|<span data-ttu-id="bab89-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bab89-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bab89-127">Request body</span></span>

<span data-ttu-id="bab89-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bab89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab89-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bab89-129">Response</span></span>

<span data-ttu-id="bab89-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bab89-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bab89-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bab89-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bab89-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bab89-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bab89-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bab89-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
```
# <a name="c"></a>[<span data-ttu-id="bab89-134">C#</span><span class="sxs-lookup"><span data-stu-id="bab89-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bab89-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bab89-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bab89-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bab89-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bab89-137">Java</span><span class="sxs-lookup"><span data-stu-id="bab89-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bab89-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bab89-138">Response</span></span>

<span data-ttu-id="bab89-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bab89-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.custodian)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians",
    "value": [
        {
            "email": "meganb@contoso.com",
            "applyHoldToSources": false,
            "status": "released",
            "createdDateTime": "2020-10-27T15:55:43.4971108Z",
            "lastModifiedDateTime": "2020-10-30T05:34:00.947558Z",
            "releasedDateTime": "2020-10-27T15:55:58.2338864Z",
            "acknowledgedDateTime": null,
            "id": "fd03ce02ecde42a58d24fcbc9ebbea3e",
            "displayName": "Megan Bowen"
        },
        {
            "email": "AdeleV@contoso.com",
            "applyHoldToSources": true,
            "status": "active",
            "createdDateTime": "2020-08-21T13:20:02.0117254Z",
            "lastModifiedDateTime": "2020-10-27T15:14:14.1244649Z",
            "releasedDateTime": null,
            "acknowledgedDateTime": null,
            "id": "2192ca408ea2410eba3bec8ae873be6b",
            "displayName": "Adele Vance"
        }
    ]
}
```
