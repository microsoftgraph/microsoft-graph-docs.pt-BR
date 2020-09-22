---
title: Obter indicador de inteligência de ameaças
description: Recupere as propriedades e os relacionamentos de um objeto tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9d6f90ef13764d3b15343a47b88489de8501a210
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076572"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="be56f-103">Obter indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="be56f-103">Get threat intelligence indicator</span></span>

<span data-ttu-id="be56f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be56f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be56f-105">Recupere as propriedades e os relacionamentos de um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="be56f-105">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be56f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be56f-106">Permissions</span></span>

<span data-ttu-id="be56f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be56f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be56f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be56f-109">Permission type</span></span>                        | <span data-ttu-id="be56f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be56f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be56f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be56f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be56f-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="be56f-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="be56f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be56f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be56f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be56f-114">Not supported.</span></span> |
| <span data-ttu-id="be56f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be56f-115">Application</span></span>                            | <span data-ttu-id="be56f-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="be56f-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="be56f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be56f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be56f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be56f-118">Optional query parameters</span></span>

<span data-ttu-id="be56f-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be56f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be56f-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="be56f-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="be56f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be56f-121">Request headers</span></span>

| <span data-ttu-id="be56f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="be56f-122">Name</span></span>      |<span data-ttu-id="be56f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="be56f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be56f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be56f-124">Authorization</span></span> | <span data-ttu-id="be56f-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="be56f-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="be56f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be56f-126">Request body</span></span>

<span data-ttu-id="be56f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be56f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be56f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="be56f-128">Response</span></span>

<span data-ttu-id="be56f-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be56f-129">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be56f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be56f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be56f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be56f-131">Request</span></span>

<span data-ttu-id="be56f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be56f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be56f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="be56f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="be56f-134">C#</span><span class="sxs-lookup"><span data-stu-id="be56f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be56f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be56f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be56f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be56f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be56f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="be56f-137">Response</span></span>

<span data-ttu-id="be56f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be56f-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="be56f-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="be56f-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be56f-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be56f-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "action": "action-value",
  "activityGroupNames": [
    "activityGroupNames-value"
  ],
  "additionalInformation": "additionalInformation-value",
  "azureTenantId": "azureTenantId-value",
  "confidence": 99,
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


