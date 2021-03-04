---
title: Listar legalHolds
description: Obter os recursos legalHold da propriedade de navegação legalHolds.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 15798da638a43f6a126c1aef6bd9e88c1015e67a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445843"
---
# <a name="list-legalholds"></a><span data-ttu-id="5eb4b-103">Listar legalHolds</span><span class="sxs-lookup"><span data-stu-id="5eb4b-103">List legalHolds</span></span>

<span data-ttu-id="5eb4b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5eb4b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eb4b-105">Obter [os legalHolds](../resources/ediscovery-legalhold.md) que são aplicados a um caso.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-105">Get the [legalHolds](../resources/ediscovery-legalhold.md) that are applied to a case.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eb4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5eb4b-106">Permissions</span></span>

<span data-ttu-id="5eb4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5eb4b-109">Permission type</span></span>|<span data-ttu-id="5eb4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5eb4b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eb4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5eb4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5eb4b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eb4b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5eb4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5eb4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eb4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-114">Not supported.</span></span>|
|<span data-ttu-id="5eb4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5eb4b-115">Application</span></span>|<span data-ttu-id="5eb4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eb4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb4b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eb4b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5eb4b-118">Optional query parameters</span></span>

<span data-ttu-id="5eb4b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5eb4b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5eb4b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eb4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb4b-121">Request headers</span></span>

|<span data-ttu-id="5eb4b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5eb4b-122">Name</span></span>|<span data-ttu-id="5eb4b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5eb4b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5eb4b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5eb4b-124">Authorization</span></span>|<span data-ttu-id="5eb4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eb4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb4b-127">Request body</span></span>

<span data-ttu-id="5eb4b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eb4b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb4b-129">Response</span></span>

<span data-ttu-id="5eb4b-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos legalHold](../resources/ediscovery-legalhold.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-130">If successful, this method returns a `200 OK` response code and a collection of [legalHold](../resources/ediscovery-legalhold.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5eb4b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5eb4b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5eb4b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb4b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
```

### <a name="response"></a><span data-ttu-id="5eb4b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb4b-133">Response</span></span>

<span data-ttu-id="5eb4b-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5eb4b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.legalHold)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```
