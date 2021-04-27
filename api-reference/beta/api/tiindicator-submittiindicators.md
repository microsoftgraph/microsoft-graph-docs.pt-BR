---
title: 'tiIndicator: submitTiIndicators'
description: Upload vários indicadores de TI (inteligência de ameaça) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: ed4ccd5adf087ecf8be69d8d192ae180ec685090
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050777"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="75d4b-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="75d4b-103">tiIndicator: submitTiIndicators</span></span>

<span data-ttu-id="75d4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75d4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75d4b-105">Upload vários indicadores de TI (inteligência de ameaça) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="75d4b-105">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="75d4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="75d4b-106">Permissions</span></span>

<span data-ttu-id="75d4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75d4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75d4b-109">Permission type</span></span> | <span data-ttu-id="75d4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75d4b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="75d4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75d4b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75d4b-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="75d4b-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="75d4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75d4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75d4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75d4b-114">Not supported.</span></span> |
| <span data-ttu-id="75d4b-115">Application</span><span class="sxs-lookup"><span data-stu-id="75d4b-115">Application</span></span>                            | <span data-ttu-id="75d4b-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="75d4b-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="75d4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75d4b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="75d4b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75d4b-118">Request headers</span></span>

| <span data-ttu-id="75d4b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="75d4b-119">Name</span></span>          | <span data-ttu-id="75d4b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="75d4b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="75d4b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="75d4b-121">Authorization</span></span> | <span data-ttu-id="75d4b-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="75d4b-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="75d4b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75d4b-123">Request body</span></span>

<span data-ttu-id="75d4b-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75d4b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75d4b-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="75d4b-125">Parameter</span></span>    | <span data-ttu-id="75d4b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="75d4b-126">Type</span></span>        | <span data-ttu-id="75d4b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="75d4b-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75d4b-128">valor</span><span class="sxs-lookup"><span data-stu-id="75d4b-128">value</span></span>|<span data-ttu-id="75d4b-129">Coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="75d4b-129">tiIndicator collection</span></span>| <span data-ttu-id="75d4b-130">Coleção JSON **de tiIndicators** a serem criados.</span><span class="sxs-lookup"><span data-stu-id="75d4b-130">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="75d4b-131">Para cada tiIndicator, fornece uma representação JSON de um objeto [tiIndicator](../resources/tiindicator.md) contendo pelo menos um [email](../resources/tiindicator.md#indicator-observables---email) [,](../resources/tiindicator.md#indicator-observables---file)arquivo ou rede observável, e os seguintes campos obrigatórios: , , , , , , , [](../resources/tiindicator.md#indicator-observables---network) `action` `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` .</span><span class="sxs-lookup"><span data-stu-id="75d4b-131">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="75d4b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="75d4b-132">Response</span></span>

<span data-ttu-id="75d4b-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75d4b-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="75d4b-134">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="75d4b-134">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="75d4b-135">Consulte [Erros para](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="75d4b-135">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="75d4b-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="75d4b-136">Examples</span></span>

<span data-ttu-id="75d4b-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="75d4b-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="75d4b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75d4b-138">Request</span></span>

<span data-ttu-id="75d4b-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="75d4b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75d4b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="75d4b-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="75d4b-141">C#</span><span class="sxs-lookup"><span data-stu-id="75d4b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75d4b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75d4b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75d4b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75d4b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75d4b-144">Java</span><span class="sxs-lookup"><span data-stu-id="75d4b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-submittiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75d4b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="75d4b-145">Response</span></span>

<span data-ttu-id="75d4b-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="75d4b-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="75d4b-147">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="75d4b-147">The response object shown here might be shortened for readability.</span></span>

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


