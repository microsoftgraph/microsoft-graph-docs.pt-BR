---
title: Listar site custodiadoSources
description: Obter uma lista dos objetos siteSource e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c51de320f3d89d37b8c0e5d38d86ea93b61f5703
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445808"
---
# <a name="list-custodian-sitesources"></a><span data-ttu-id="0180e-103">Listar site custodiadoSources</span><span class="sxs-lookup"><span data-stu-id="0180e-103">List custodian siteSources</span></span>

<span data-ttu-id="0180e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0180e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0180e-105">Obter uma lista de [objetos siteSource](../resources/ediscovery-sitesource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0180e-105">Get a list of [siteSource](../resources/ediscovery-sitesource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0180e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0180e-106">Permissions</span></span>

<span data-ttu-id="0180e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0180e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0180e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0180e-109">Permission type</span></span>|<span data-ttu-id="0180e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0180e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0180e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0180e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0180e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0180e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0180e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0180e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0180e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0180e-114">Not supported.</span></span>|
|<span data-ttu-id="0180e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0180e-115">Application</span></span>|<span data-ttu-id="0180e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0180e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0180e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0180e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0180e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0180e-118">Optional query parameters</span></span>

<span data-ttu-id="0180e-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0180e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0180e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0180e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0180e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0180e-121">Request headers</span></span>

|<span data-ttu-id="0180e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0180e-122">Name</span></span>|<span data-ttu-id="0180e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0180e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0180e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0180e-124">Authorization</span></span>|<span data-ttu-id="0180e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0180e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0180e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0180e-127">Request body</span></span>

<span data-ttu-id="0180e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0180e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0180e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0180e-129">Response</span></span>

<span data-ttu-id="0180e-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0180e-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0180e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0180e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0180e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0180e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
```

### <a name="response"></a><span data-ttu-id="0180e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0180e-133">Response</span></span>

<span data-ttu-id="0180e-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0180e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
