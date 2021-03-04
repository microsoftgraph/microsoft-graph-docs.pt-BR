---
title: Listar sourceCollections
description: Obter a lista de recursos sourceCollections de um objeto case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 10f474b98d8ecde7d12b353ae0bedb4bcebed749
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445838"
---
# <a name="list-sourcecollections"></a><span data-ttu-id="81675-103">Listar sourceCollections</span><span class="sxs-lookup"><span data-stu-id="81675-103">List sourceCollections</span></span>

<span data-ttu-id="81675-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="81675-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81675-105">Obter a lista [de sourceCollections](../resources/ediscovery-sourcecollection.md) de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="81675-105">Get the list of [sourceCollections](../resources/ediscovery-sourcecollection.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81675-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81675-106">Permissions</span></span>

<span data-ttu-id="81675-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81675-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81675-109">Permission type</span></span>|<span data-ttu-id="81675-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81675-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81675-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81675-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81675-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81675-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="81675-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81675-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81675-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81675-114">Not supported.</span></span>|
|<span data-ttu-id="81675-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81675-115">Application</span></span>|<span data-ttu-id="81675-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81675-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81675-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81675-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81675-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81675-118">Optional query parameters</span></span>

<span data-ttu-id="81675-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81675-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="81675-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="81675-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="81675-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81675-121">Request headers</span></span>

|<span data-ttu-id="81675-122">Nome</span><span class="sxs-lookup"><span data-stu-id="81675-122">Name</span></span>|<span data-ttu-id="81675-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="81675-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81675-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="81675-124">Authorization</span></span>|<span data-ttu-id="81675-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81675-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81675-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81675-127">Request body</span></span>

<span data-ttu-id="81675-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81675-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81675-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="81675-129">Response</span></span>

<span data-ttu-id="81675-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81675-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81675-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81675-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81675-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81675-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections
```

### <a name="response"></a><span data-ttu-id="81675-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81675-133">Response</span></span>

<span data-ttu-id="81675-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81675-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
