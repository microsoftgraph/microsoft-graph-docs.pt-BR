---
title: Listar unifiedGroupSources
description: Obter uma lista dos objetos unifiedGroupSource e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7f657981d295396098d676a21069f8f11df52e0b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445807"
---
# <a name="list-unifiedgroupsources"></a><span data-ttu-id="800a8-103">Listar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="800a8-103">List unifiedGroupSources</span></span>

<span data-ttu-id="800a8-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="800a8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="800a8-105">Obter uma lista dos [objetos unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="800a8-105">Get a list of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="800a8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="800a8-106">Permissions</span></span>

<span data-ttu-id="800a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="800a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="800a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="800a8-109">Permission type</span></span>|<span data-ttu-id="800a8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="800a8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="800a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="800a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="800a8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800a8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="800a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="800a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="800a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="800a8-114">Not supported.</span></span>|
|<span data-ttu-id="800a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="800a8-115">Application</span></span>|<span data-ttu-id="800a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="800a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="800a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="800a8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="800a8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="800a8-118">Optional query parameters</span></span>

<span data-ttu-id="800a8-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="800a8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="800a8-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="800a8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="800a8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="800a8-121">Request headers</span></span>

|<span data-ttu-id="800a8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="800a8-122">Name</span></span>|<span data-ttu-id="800a8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="800a8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="800a8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="800a8-124">Authorization</span></span>|<span data-ttu-id="800a8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="800a8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="800a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="800a8-127">Request body</span></span>

<span data-ttu-id="800a8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="800a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="800a8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="800a8-129">Response</span></span>

<span data-ttu-id="800a8-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="800a8-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="800a8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="800a8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="800a8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="800a8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="800a8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="800a8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```
# <a name="c"></a>[<span data-ttu-id="800a8-134">C#</span><span class="sxs-lookup"><span data-stu-id="800a8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="800a8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="800a8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="800a8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="800a8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="800a8-137">Java</span><span class="sxs-lookup"><span data-stu-id="800a8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="800a8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="800a8-138">Response</span></span>

<span data-ttu-id="800a8-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="800a8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.unifiedGroupSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "Megan Bowen"
                }
            }
        }
    ]
}
```
