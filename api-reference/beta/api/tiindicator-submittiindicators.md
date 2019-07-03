---
title: 'tiIndicator: submitTiIndicators'
description: Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 199e004dc185fa466843fe49ef4736f81a74c594
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451406"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="5e930-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="5e930-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e930-104">Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="5e930-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e930-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e930-105">Permissions</span></span>

<span data-ttu-id="5e930-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e930-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e930-108">Permission type</span></span> | <span data-ttu-id="5e930-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e930-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5e930-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e930-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e930-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="5e930-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="5e930-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e930-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e930-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e930-113">Not supported.</span></span> |
| <span data-ttu-id="5e930-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e930-114">Application</span></span>                            | <span data-ttu-id="5e930-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="5e930-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e930-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e930-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="5e930-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e930-117">Request headers</span></span>

| <span data-ttu-id="5e930-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5e930-118">Name</span></span>          | <span data-ttu-id="5e930-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e930-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5e930-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e930-120">Authorization</span></span> | <span data-ttu-id="5e930-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5e930-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e930-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e930-122">Request body</span></span>

<span data-ttu-id="5e930-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e930-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e930-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5e930-124">Parameter</span></span>    | <span data-ttu-id="5e930-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e930-125">Type</span></span>        | <span data-ttu-id="5e930-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e930-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e930-127">valor</span><span class="sxs-lookup"><span data-stu-id="5e930-127">value</span></span>|<span data-ttu-id="5e930-128">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="5e930-128">tiIndicator collection</span></span>| <span data-ttu-id="5e930-129">Coleção JSON de **tiIndicators** a ser criada.</span><span class="sxs-lookup"><span data-stu-id="5e930-129">JSON collection of **tiIndicators** to be created.</span></span> |

## <a name="response"></a><span data-ttu-id="5e930-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e930-130">Response</span></span>

<span data-ttu-id="5e930-131">Se bem-sucedido, este método retorna `200, OK` o código de resposta e um objeto da coleção [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e930-131">If successful, this method returns `200, OK` response code and a [tiIndicator](../resources/tiindicator.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e930-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5e930-132">Examples</span></span>

<span data-ttu-id="5e930-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5e930-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5e930-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e930-134">Request</span></span>

<span data-ttu-id="5e930-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e930-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e930-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e930-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e930-137">C#</span><span class="sxs-lookup"><span data-stu-id="5e930-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e930-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e930-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e930-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5e930-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e930-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e930-140">Response</span></span>

<span data-ttu-id="5e930-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e930-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5e930-142">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e930-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e930-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e930-143">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: submitTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
