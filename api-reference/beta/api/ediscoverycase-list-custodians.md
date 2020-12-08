---
title: Listar os responsáveis
description: Obtenha uma lista dos objetos responsáveis e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 394d02a8761e2911343996723673b230a4a6fe01
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597521"
---
# <a name="list-custodians"></a><span data-ttu-id="c598b-103">Listar os responsáveis</span><span class="sxs-lookup"><span data-stu-id="c598b-103">List custodians</span></span>

<span data-ttu-id="c598b-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c598b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c598b-105">Obtenha uma lista dos objetos [responsáveis](../resources/custodian.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c598b-105">Get a list of the [custodian](../resources/custodian.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c598b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c598b-106">Permissions</span></span>

<span data-ttu-id="c598b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c598b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c598b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c598b-109">Permission type</span></span>|<span data-ttu-id="c598b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c598b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c598b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c598b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c598b-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c598b-112">User.Read</span></span>|
|<span data-ttu-id="c598b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c598b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c598b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c598b-114">Not supported.</span></span>|
|<span data-ttu-id="c598b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c598b-115">Application</span></span>|<span data-ttu-id="c598b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c598b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c598b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c598b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c598b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c598b-118">Optional query parameters</span></span>

<span data-ttu-id="c598b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c598b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c598b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c598b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c598b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c598b-121">Request headers</span></span>

|<span data-ttu-id="c598b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c598b-122">Name</span></span>|<span data-ttu-id="c598b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c598b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c598b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c598b-124">Authorization</span></span>|<span data-ttu-id="c598b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c598b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c598b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c598b-127">Request body</span></span>

<span data-ttu-id="c598b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c598b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c598b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c598b-129">Response</span></span>

<span data-ttu-id="c598b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [responsáveis](../resources/custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c598b-130">If successful, this method returns a `200 OK` response code and a collection of [custodian](../resources/custodian.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c598b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c598b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c598b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c598b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
```

### <a name="response"></a><span data-ttu-id="c598b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c598b-133">Response</span></span>

<span data-ttu-id="c598b-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c598b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.custodian)"
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
