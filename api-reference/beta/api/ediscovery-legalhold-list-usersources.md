---
title: Listar legalHold userSources
description: Obter os recursos userSource da propriedade de navegação userSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a87ff92ea60c4d7c048dff91f5fb13c92e040d11
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445787"
---
# <a name="list-legalhold-usersources"></a><span data-ttu-id="d3161-103">Listar legalHold userSources</span><span class="sxs-lookup"><span data-stu-id="d3161-103">List legalHold userSources</span></span>

<span data-ttu-id="d3161-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d3161-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3161-105">Obter a lista de [objetos userSource](../resources/ediscovery-usersource.md) associados a uma responsabilidade legal.</span><span class="sxs-lookup"><span data-stu-id="d3161-105">Get the list of [userSource](../resources/ediscovery-usersource.md) objects associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3161-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3161-106">Permissions</span></span>

<span data-ttu-id="d3161-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3161-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3161-109">Permission type</span></span>|<span data-ttu-id="d3161-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3161-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3161-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3161-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3161-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3161-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d3161-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3161-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3161-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3161-114">Not supported.</span></span>|
|<span data-ttu-id="d3161-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3161-115">Application</span></span>|<span data-ttu-id="d3161-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3161-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3161-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3161-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3161-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3161-118">Optional query parameters</span></span>

<span data-ttu-id="d3161-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3161-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d3161-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d3161-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3161-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3161-121">Request headers</span></span>

|<span data-ttu-id="d3161-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d3161-122">Name</span></span>|<span data-ttu-id="d3161-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3161-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3161-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3161-124">Authorization</span></span>|<span data-ttu-id="d3161-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3161-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3161-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3161-127">Request body</span></span>

<span data-ttu-id="d3161-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3161-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3161-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3161-129">Response</span></span>

<span data-ttu-id="d3161-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3161-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3161-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3161-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3161-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3161-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/userSources
```

### <a name="response"></a><span data-ttu-id="d3161-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3161-133">Response</span></span>

<span data-ttu-id="d3161-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3161-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalholds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "2f279b24-2142-435d-97c5-0d42220ba453",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
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
