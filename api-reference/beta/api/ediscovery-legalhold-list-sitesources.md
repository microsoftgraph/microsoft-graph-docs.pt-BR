---
title: Listar legalHold siteSources
description: Obter a lista de objetos siteSource associados a uma resserção legal.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2e3be09db4a31a4bb8a3edf86194712f3aa4416c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445788"
---
# <a name="list-legalhold-sitesources"></a><span data-ttu-id="af439-103">Listar legalHold siteSources</span><span class="sxs-lookup"><span data-stu-id="af439-103">List legalHold siteSources</span></span>

<span data-ttu-id="af439-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="af439-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af439-105">Obter a lista [de objetos siteSource](../resources/ediscovery-sitesource.md) associados a uma resserção legal.</span><span class="sxs-lookup"><span data-stu-id="af439-105">Get the list of [siteSource](../resources/ediscovery-sitesource.md) objecs associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="af439-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af439-106">Permissions</span></span>

<span data-ttu-id="af439-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions- reference).</span><span class="sxs-lookup"><span data-stu-id="af439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions- reference).</span></span>

|<span data-ttu-id="af439-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af439-109">Permission type</span></span>|<span data-ttu-id="af439-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af439-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af439-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af439-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af439-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af439-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="af439-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af439-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af439-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af439-114">Not supported.</span></span>|
|<span data-ttu-id="af439-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af439-115">Application</span></span>|<span data-ttu-id="af439-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af439-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af439-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af439-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af439-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af439-118">Optional query parameters</span></span>

<span data-ttu-id="af439-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af439-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="af439-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="af439-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="af439-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af439-121">Request headers</span></span>

|<span data-ttu-id="af439-122">Nome</span><span class="sxs-lookup"><span data-stu-id="af439-122">Name</span></span>|<span data-ttu-id="af439-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="af439-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af439-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="af439-124">Authorization</span></span>|<span data-ttu-id="af439-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af439-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af439-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af439-127">Request body</span></span>

<span data-ttu-id="af439-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af439-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af439-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="af439-129">Response</span></span>

<span data-ttu-id="af439-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af439-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af439-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af439-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af439-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af439-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources
```

### <a name="response"></a><span data-ttu-id="af439-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af439-133">Response</span></span>

<span data-ttu-id="af439-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="af439-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "43aab990-183e-4593-b772-578bb129e89b",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        },
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "e87b37ac-fad4-471b-9dd8-0e16000a3554",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
