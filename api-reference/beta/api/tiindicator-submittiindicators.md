---
title: 'tiIndicator: submitTiIndicators'
description: Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d2cda5dd77124d96139cde568d6d88ac4d167dde
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219724"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="e4989-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="e4989-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4989-104">Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="e4989-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4989-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4989-105">Permissions</span></span>

<span data-ttu-id="e4989-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4989-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4989-108">Permission type</span></span> | <span data-ttu-id="e4989-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4989-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e4989-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4989-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4989-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e4989-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e4989-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4989-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4989-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4989-113">Not supported.</span></span> |
| <span data-ttu-id="e4989-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4989-114">Application</span></span>                            | <span data-ttu-id="e4989-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e4989-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4989-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4989-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="e4989-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4989-117">Request headers</span></span>

| <span data-ttu-id="e4989-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e4989-118">Name</span></span>          | <span data-ttu-id="e4989-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4989-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e4989-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4989-120">Authorization</span></span> | <span data-ttu-id="e4989-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e4989-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4989-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4989-122">Request body</span></span>

<span data-ttu-id="e4989-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4989-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e4989-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e4989-124">Parameter</span></span>    | <span data-ttu-id="e4989-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4989-125">Type</span></span>        | <span data-ttu-id="e4989-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4989-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e4989-127">valor</span><span class="sxs-lookup"><span data-stu-id="e4989-127">value</span></span>|<span data-ttu-id="e4989-128">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="e4989-128">tiIndicator collection</span></span>| <span data-ttu-id="e4989-129">Coleção JSON de **tiIndicators** a ser criada.</span><span class="sxs-lookup"><span data-stu-id="e4989-129">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="e4989-130">Para cada tiIndicator, forneça uma representação JSON de um objeto [tiIndicator](../resources/tiindicator.md) que contém pelo menos [um email](../resources/tiindicator.md#indicator-observables---email), [arquivo](../resources/tiindicator.md#indicator-observables---file)ou [rede](../resources/tiindicator.md#indicator-observables---network) observou, e os seguintes campos obrigatórios `description`: `expirationDateTime` `action`, `targetProduct`, `threatType`, `tlpLevel`,,.</span><span class="sxs-lookup"><span data-stu-id="e4989-130">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="e4989-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4989-131">Response</span></span>

<span data-ttu-id="e4989-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4989-132">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="e4989-133">Se houver um erro, este método retornará um código `206 Partial Content` de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4989-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="e4989-134">Consulte [erros](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e4989-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="e4989-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e4989-135">Examples</span></span>

<span data-ttu-id="e4989-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e4989-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e4989-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4989-137">Request</span></span>

<span data-ttu-id="e4989-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4989-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4989-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4989-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e4989-140">C#</span><span class="sxs-lookup"><span data-stu-id="e4989-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4989-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4989-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4989-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4989-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4989-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4989-143">Response</span></span>

<span data-ttu-id="e4989-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4989-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e4989-145">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4989-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e4989-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4989-146">All the properties will be returned from an actual call.</span></span>

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
