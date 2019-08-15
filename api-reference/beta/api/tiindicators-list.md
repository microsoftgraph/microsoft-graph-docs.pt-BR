---
title: Listar indicadores de inteligência de ameaças
description: Recupere uma lista de objetos tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7f0bc8de6ad01a837317f4512aadc88b0b43bd72
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409272"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="9a942-103">Listar indicadores de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="9a942-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a942-104">Recupere uma lista de objetos [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="9a942-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a942-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a942-105">Permissions</span></span>

<span data-ttu-id="9a942-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a942-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a942-108">Permission type</span></span>     | <span data-ttu-id="9a942-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a942-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a942-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a942-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a942-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9a942-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="9a942-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a942-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a942-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a942-113">Not supported.</span></span> |
| <span data-ttu-id="9a942-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a942-114">Application</span></span>                            | <span data-ttu-id="9a942-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9a942-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a942-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a942-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a942-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a942-117">Optional query parameters</span></span>

<span data-ttu-id="9a942-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a942-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9a942-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9a942-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a942-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a942-120">Request headers</span></span>

| <span data-ttu-id="9a942-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9a942-121">Name</span></span>      |<span data-ttu-id="9a942-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a942-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a942-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a942-123">Authorization</span></span> | <span data-ttu-id="9a942-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9a942-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a942-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a942-125">Request body</span></span>

<span data-ttu-id="9a942-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a942-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a942-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a942-127">Response</span></span>

<span data-ttu-id="9a942-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a942-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a942-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a942-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a942-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a942-130">Request</span></span>

<span data-ttu-id="9a942-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a942-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a942-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a942-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a942-133">C#</span><span class="sxs-lookup"><span data-stu-id="9a942-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a942-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a942-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a942-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9a942-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a942-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a942-136">Response</span></span>

<span data-ttu-id="9a942-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a942-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9a942-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a942-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9a942-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a942-139">All the properties will be returned from an actual call.</span></span>

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
