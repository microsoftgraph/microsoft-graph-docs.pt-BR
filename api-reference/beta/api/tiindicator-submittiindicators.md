---
title: 'tiIndicator: submitTiIndicators'
description: Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 944b6d3617f8a850e1f2ac3f681076984edd6c7a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637553"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="cb13d-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="cb13d-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb13d-104">Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="cb13d-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb13d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb13d-105">Permissions</span></span>

<span data-ttu-id="cb13d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb13d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb13d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb13d-108">Permission type</span></span> | <span data-ttu-id="cb13d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb13d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb13d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb13d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb13d-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cb13d-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="cb13d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb13d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb13d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb13d-113">Not supported.</span></span> |
| <span data-ttu-id="cb13d-114">Application</span><span class="sxs-lookup"><span data-stu-id="cb13d-114">Application</span></span>                            | <span data-ttu-id="cb13d-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cb13d-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb13d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb13d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="cb13d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb13d-117">Request headers</span></span>

| <span data-ttu-id="cb13d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cb13d-118">Name</span></span>          | <span data-ttu-id="cb13d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb13d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cb13d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb13d-120">Authorization</span></span> | <span data-ttu-id="cb13d-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cb13d-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb13d-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb13d-122">Request body</span></span>

<span data-ttu-id="cb13d-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb13d-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb13d-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cb13d-124">Parameter</span></span>    | <span data-ttu-id="cb13d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb13d-125">Type</span></span>        | <span data-ttu-id="cb13d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb13d-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb13d-127">valor</span><span class="sxs-lookup"><span data-stu-id="cb13d-127">value</span></span>|<span data-ttu-id="cb13d-128">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="cb13d-128">tiIndicator collection</span></span>| <span data-ttu-id="cb13d-129">Coleção JSON de **tiIndicators** a ser criada.</span><span class="sxs-lookup"><span data-stu-id="cb13d-129">JSON collection of **tiIndicators** to be created.</span></span> |

## <a name="response"></a><span data-ttu-id="cb13d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb13d-130">Response</span></span>

<span data-ttu-id="cb13d-131">Se bem-sucedido, este método retorna `200, OK` o código de resposta e um objeto da coleção [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb13d-131">If successful, this method returns `200, OK` response code and a [tiIndicator](../resources/tiindicator.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb13d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb13d-132">Examples</span></span>

<span data-ttu-id="cb13d-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cb13d-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cb13d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb13d-134">Request</span></span>

<span data-ttu-id="cb13d-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb13d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-Type: application/json

{
  "value": [
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1668987+00:00",
      "externalId": "Test--8586509942423126760MS164-0",
      "fileHashType": "sha256",
      "fileHashValue": "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    },
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1748779+00:00",
      "externalId": "Test--8586509942423126760MS164-1",
      "fileHashType": "sha256",
      "fileHashValue": "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cb13d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb13d-136">Response</span></span>

<span data-ttu-id="cb13d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb13d-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cb13d-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cb13d-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb13d-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb13d-139">All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": null,
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cb13d-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cb13d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cb13d-141">Basic</span><span class="sxs-lookup"><span data-stu-id="cb13d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_submittiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb13d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb13d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_submittiindicators-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: submitTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-submittiindicators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-submittiindicators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
