---
title: Listar reviewSets
description: Obter os recursos reviewSet de um objeto case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: eb881a041ac890cb5c2c616cbf57189e26f8e272
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445840"
---
# <a name="list-reviewsets"></a><span data-ttu-id="f3d61-103">Listar reviewSets</span><span class="sxs-lookup"><span data-stu-id="f3d61-103">List reviewSets</span></span>

<span data-ttu-id="f3d61-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f3d61-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3d61-105">Obter a lista de [reviewSets](../resources/ediscovery-reviewset.md) de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="f3d61-105">Get the list of [reviewSets](../resources/ediscovery-reviewset.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3d61-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3d61-106">Permissions</span></span>

<span data-ttu-id="f3d61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3d61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3d61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3d61-109">Permission type</span></span>|<span data-ttu-id="f3d61-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3d61-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3d61-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3d61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3d61-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3d61-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f3d61-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3d61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3d61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3d61-114">Not supported.</span></span>|
|<span data-ttu-id="f3d61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3d61-115">Application</span></span>|<span data-ttu-id="f3d61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3d61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3d61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3d61-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/reviewSets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3d61-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f3d61-118">Optional query parameters</span></span>

<span data-ttu-id="f3d61-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3d61-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f3d61-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f3d61-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3d61-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d61-121">Request headers</span></span>

|<span data-ttu-id="f3d61-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f3d61-122">Name</span></span>|<span data-ttu-id="f3d61-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3d61-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f3d61-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3d61-124">Authorization</span></span>|<span data-ttu-id="f3d61-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3d61-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3d61-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d61-127">Request body</span></span>

<span data-ttu-id="f3d61-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3d61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3d61-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3d61-129">Response</span></span>

<span data-ttu-id="f3d61-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3d61-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3d61-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f3d61-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3d61-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d61-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/reviewSets
```

### <a name="response"></a><span data-ttu-id="f3d61-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3d61-133">Response</span></span>

<span data-ttu-id="f3d61-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f3d61-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
