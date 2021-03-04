---
title: Listar operações
description: Obter a lista caseOperations de um objeto case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6f6cd402a88f0ce10e963cab0e3c0d94549f0dbd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445842"
---
# <a name="list-operations"></a><span data-ttu-id="004ec-103">Listar operações</span><span class="sxs-lookup"><span data-stu-id="004ec-103">List operations</span></span>

<span data-ttu-id="004ec-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="004ec-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="004ec-105">Obter a lista [de caseOperations](../resources/ediscovery-caseoperation.md) de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="004ec-105">Get the list of [caseOperations](../resources/ediscovery-caseoperation.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="004ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="004ec-106">Permissions</span></span>

<span data-ttu-id="004ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="004ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="004ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="004ec-109">Permission type</span></span>|<span data-ttu-id="004ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="004ec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="004ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="004ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="004ec-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004ec-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="004ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="004ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="004ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="004ec-114">Not supported.</span></span>|
|<span data-ttu-id="004ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="004ec-115">Application</span></span>|<span data-ttu-id="004ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="004ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="004ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="004ec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="004ec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="004ec-118">Optional query parameters</span></span>

<span data-ttu-id="004ec-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="004ec-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="004ec-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="004ec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="004ec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="004ec-121">Request headers</span></span>

|<span data-ttu-id="004ec-122">Nome</span><span class="sxs-lookup"><span data-stu-id="004ec-122">Name</span></span>|<span data-ttu-id="004ec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="004ec-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="004ec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="004ec-124">Authorization</span></span>|<span data-ttu-id="004ec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="004ec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="004ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="004ec-127">Request body</span></span>
<span data-ttu-id="004ec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="004ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="004ec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="004ec-129">Response</span></span>

<span data-ttu-id="004ec-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="004ec-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="004ec-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="004ec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="004ec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="004ec-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_caseoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations
```

### <a name="response"></a><span data-ttu-id="004ec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="004ec-133">Response</span></span>

<span data-ttu-id="004ec-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="004ec-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.caseOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
      "id": "41362b70-2b70-4136-702b-3641702b3641",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
