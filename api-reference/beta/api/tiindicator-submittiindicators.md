---
title: 'tiIndicator: submitTiIndicators'
description: Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 319c529f567150914a6050da85fb6a9379c4f1a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076502"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="9b869-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="9b869-103">tiIndicator: submitTiIndicators</span></span>

<span data-ttu-id="9b869-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b869-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b869-105">Carregar vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="9b869-105">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b869-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b869-106">Permissions</span></span>

<span data-ttu-id="9b869-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b869-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b869-109">Permission type</span></span> | <span data-ttu-id="9b869-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b869-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b869-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b869-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b869-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9b869-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="9b869-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b869-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b869-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b869-114">Not supported.</span></span> |
| <span data-ttu-id="9b869-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b869-115">Application</span></span>                            | <span data-ttu-id="9b869-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9b869-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b869-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b869-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="9b869-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b869-118">Request headers</span></span>

| <span data-ttu-id="9b869-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9b869-119">Name</span></span>          | <span data-ttu-id="9b869-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b869-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9b869-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b869-121">Authorization</span></span> | <span data-ttu-id="9b869-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9b869-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b869-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b869-123">Request body</span></span>

<span data-ttu-id="9b869-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b869-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b869-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9b869-125">Parameter</span></span>    | <span data-ttu-id="9b869-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b869-126">Type</span></span>        | <span data-ttu-id="9b869-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b869-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b869-128">valor</span><span class="sxs-lookup"><span data-stu-id="9b869-128">value</span></span>|<span data-ttu-id="9b869-129">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="9b869-129">tiIndicator collection</span></span>| <span data-ttu-id="9b869-130">Coleção JSON de **tiIndicators** a ser criada.</span><span class="sxs-lookup"><span data-stu-id="9b869-130">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="9b869-131">Para cada tiIndicator, forneça uma representação JSON de um objeto [tiIndicator](../resources/tiindicator.md) que contém pelo menos um [email](../resources/tiindicator.md#indicator-observables---email), [arquivo](../resources/tiindicator.md#indicator-observables---file)ou [rede](../resources/tiindicator.md#indicator-observables---network) observou, e os seguintes campos obrigatórios:,,,, `action` `description` `expirationDateTime` `targetProduct` `threatType` , `tlpLevel` .</span><span class="sxs-lookup"><span data-stu-id="9b869-131">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="9b869-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b869-132">Response</span></span>

<span data-ttu-id="9b869-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b869-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="9b869-134">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b869-134">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="9b869-135">Consulte [erros](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="9b869-135">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="9b869-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b869-136">Examples</span></span>

<span data-ttu-id="9b869-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9b869-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9b869-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b869-138">Request</span></span>

<span data-ttu-id="9b869-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b869-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b869-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b869-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9b869-141">C#</span><span class="sxs-lookup"><span data-stu-id="9b869-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b869-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b869-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b869-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b869-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b869-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b869-144">Response</span></span>

<span data-ttu-id="9b869-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b869-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9b869-146">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9b869-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9b869-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b869-147">All the properties will be returned from an actual call.</span></span>

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


