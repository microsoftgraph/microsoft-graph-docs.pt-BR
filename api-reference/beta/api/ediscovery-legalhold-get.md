---
title: Obter legalHold
description: Leia as propriedades e as relações de um objeto legalHold.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f2d276a85a6f95b845acef48fc3e823cb08be79b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445789"
---
# <a name="get-legalhold"></a><span data-ttu-id="6bac4-103">Obter legalHold</span><span class="sxs-lookup"><span data-stu-id="6bac4-103">Get legalHold</span></span>

<span data-ttu-id="6bac4-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6bac4-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bac4-105">Leia as propriedades e as relações de um [objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="6bac4-105">Read the properties and relationships of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bac4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bac4-106">Permissions</span></span>

<span data-ttu-id="6bac4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bac4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bac4-109">Permission type</span></span>|<span data-ttu-id="6bac4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bac4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bac4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bac4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bac4-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bac4-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6bac4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bac4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bac4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bac4-114">Not supported.</span></span>|
|<span data-ttu-id="6bac4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bac4-115">Application</span></span>|<span data-ttu-id="6bac4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bac4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bac4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bac4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6bac4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6bac4-118">Optional query parameters</span></span>

<span data-ttu-id="6bac4-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6bac4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6bac4-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6bac4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bac4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bac4-121">Request headers</span></span>

|<span data-ttu-id="6bac4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6bac4-122">Name</span></span>|<span data-ttu-id="6bac4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bac4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6bac4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bac4-124">Authorization</span></span>|<span data-ttu-id="6bac4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bac4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bac4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bac4-127">Request body</span></span>

<span data-ttu-id="6bac4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6bac4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bac4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bac4-129">Response</span></span>

<span data-ttu-id="6bac4-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bac4-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bac4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6bac4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6bac4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bac4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

### <a name="response"></a><span data-ttu-id="6bac4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bac4-133">Response</span></span>

<span data-ttu-id="6bac4-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6bac4-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.ediscovery.legalHold",
    "id": "700cd868-d868-700c-68d8-0c7068d80c70",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "isEnabled": "Boolean",
    "status": "String",
    "contentQuery": "String",
    "errors": [
      "String"
    ],
    "displayName": "String",
    "createdDateTime": "String (timestamp)"
  }
}
```
