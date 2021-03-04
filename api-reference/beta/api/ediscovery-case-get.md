---
title: Obter caso
description: Recupere as propriedades e as relações de um objeto case.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ed5db0f3f402ff8746d21457efe392dec728c3d8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445847"
---
# <a name="get-case"></a><span data-ttu-id="94f8f-103">Obter caso</span><span class="sxs-lookup"><span data-stu-id="94f8f-103">Get case</span></span>

<span data-ttu-id="94f8f-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="94f8f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94f8f-105">Recupere as propriedades e as relações de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="94f8f-105">Retrieve the properties and relationships of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94f8f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94f8f-106">Permissions</span></span>

<span data-ttu-id="94f8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f8f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94f8f-109">Permission type</span></span>|<span data-ttu-id="94f8f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94f8f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f8f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94f8f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94f8f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f8f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="94f8f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94f8f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f8f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94f8f-114">Not supported.</span></span>|
|<span data-ttu-id="94f8f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94f8f-115">Application</span></span>|<span data-ttu-id="94f8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94f8f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f8f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94f8f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94f8f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94f8f-118">Optional query parameters</span></span>

<span data-ttu-id="94f8f-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94f8f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="94f8f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94f8f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94f8f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94f8f-121">Request headers</span></span>

| <span data-ttu-id="94f8f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="94f8f-122">Name</span></span>      |<span data-ttu-id="94f8f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f8f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94f8f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="94f8f-124">Authorization</span></span> | <span data-ttu-id="94f8f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94f8f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94f8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94f8f-127">Request body</span></span>

<span data-ttu-id="94f8f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94f8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94f8f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94f8f-129">Response</span></span>

<span data-ttu-id="94f8f-130">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94f8f-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94f8f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94f8f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94f8f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94f8f-132">Request</span></span>

<span data-ttu-id="94f8f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94f8f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_case"
}-->

```http
GET https://graph.microsoft.com/beta/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

### <a name="response"></a><span data-ttu-id="94f8f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="94f8f-134">Response</span></span>

<span data-ttu-id="94f8f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94f8f-135">The following is an example of the response.</span></span>

> <span data-ttu-id="94f8f-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94f8f-136">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
