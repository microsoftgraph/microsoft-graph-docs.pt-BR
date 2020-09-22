---
title: Listar indicadores de inteligência de ameaças
description: Recupere uma lista de objetos tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a4040e28dea4f92e803445e4bcead8d515a76c07
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076503"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="f1f37-103">Listar indicadores de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="f1f37-103">List threat intelligence indicators</span></span>

<span data-ttu-id="f1f37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1f37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f37-105">Recupere uma lista de objetos [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="f1f37-105">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1f37-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1f37-106">Permissions</span></span>

<span data-ttu-id="f1f37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1f37-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1f37-109">Permission type</span></span>     | <span data-ttu-id="f1f37-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1f37-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1f37-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1f37-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1f37-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f1f37-112">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="f1f37-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1f37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1f37-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f37-114">Not supported.</span></span> |
| <span data-ttu-id="f1f37-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1f37-115">Application</span></span>                            | <span data-ttu-id="f1f37-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f1f37-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1f37-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f37-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1f37-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1f37-118">Optional query parameters</span></span>

<span data-ttu-id="f1f37-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1f37-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f1f37-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f1f37-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1f37-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f37-121">Request headers</span></span>

| <span data-ttu-id="f1f37-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f1f37-122">Name</span></span>      |<span data-ttu-id="f1f37-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f37-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1f37-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1f37-124">Authorization</span></span> | <span data-ttu-id="f1f37-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f1f37-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1f37-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f37-126">Request body</span></span>

<span data-ttu-id="f1f37-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1f37-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1f37-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f37-128">Response</span></span>

<span data-ttu-id="f1f37-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1f37-129">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1f37-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1f37-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1f37-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f37-131">Request</span></span>

<span data-ttu-id="f1f37-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1f37-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1f37-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f37-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators
```
# <a name="c"></a>[<span data-ttu-id="f1f37-134">C#</span><span class="sxs-lookup"><span data-stu-id="f1f37-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1f37-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1f37-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1f37-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1f37-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1f37-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f37-137">Response</span></span>

<span data-ttu-id="f1f37-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1f37-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f1f37-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1f37-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1f37-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1f37-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


