---
title: 'tiIndicator: updateTiIndicators'
description: Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0be11755ff976037ab593c3273ed70b30eb4e4dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076504"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="e0a32-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="e0a32-103">tiIndicator: updateTiIndicators</span></span>

<span data-ttu-id="e0a32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0a32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a32-105">Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="e0a32-105">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0a32-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0a32-106">Permissions</span></span>

<span data-ttu-id="e0a32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0a32-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0a32-109">Permission type</span></span>   | <span data-ttu-id="e0a32-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0a32-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0a32-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0a32-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0a32-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e0a32-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e0a32-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0a32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0a32-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0a32-114">Not supported.</span></span> |
| <span data-ttu-id="e0a32-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0a32-115">Application</span></span>                            | <span data-ttu-id="e0a32-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e0a32-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0a32-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a32-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="e0a32-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a32-118">Request headers</span></span>

| <span data-ttu-id="e0a32-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0a32-119">Name</span></span>          | <span data-ttu-id="e0a32-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a32-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e0a32-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0a32-121">Authorization</span></span> | <span data-ttu-id="e0a32-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e0a32-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0a32-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a32-123">Request body</span></span>

<span data-ttu-id="e0a32-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0a32-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="e0a32-125">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update tiIndicator](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="e0a32-125">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="e0a32-126">Os campos obrigatórios para cada tiIndicator são: `id` , `expirationDateTime` , `targetProduct` .</span><span class="sxs-lookup"><span data-stu-id="e0a32-126">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="e0a32-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e0a32-127">Parameter</span></span>    | <span data-ttu-id="e0a32-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0a32-128">Type</span></span>        | <span data-ttu-id="e0a32-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a32-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0a32-130">valor</span><span class="sxs-lookup"><span data-stu-id="e0a32-130">value</span></span>|<span data-ttu-id="e0a32-131">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="e0a32-131">tiIndicator collection</span></span>| <span data-ttu-id="e0a32-132">Coleção de **tiIndicators** para atualizar.</span><span class="sxs-lookup"><span data-stu-id="e0a32-132">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="e0a32-133">Cada entidade deve ter **ID** e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e0a32-133">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="e0a32-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0a32-134">Response</span></span>

<span data-ttu-id="e0a32-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0a32-135">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="e0a32-136">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0a32-136">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="e0a32-137">Consulte [erros](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e0a32-137">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="e0a32-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0a32-138">Examples</span></span>

<span data-ttu-id="e0a32-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e0a32-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e0a32-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a32-140">Request</span></span>

<span data-ttu-id="e0a32-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0a32-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0a32-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a32-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators",
  "isCollection":true
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```
# <a name="c"></a>[<span data-ttu-id="e0a32-143">C#</span><span class="sxs-lookup"><span data-stu-id="e0a32-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0a32-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0a32-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0a32-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0a32-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0a32-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0a32-146">Response</span></span>

<span data-ttu-id="e0a32-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0a32-147">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e0a32-148">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e0a32-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e0a32-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0a32-149">All the properties will be returned from an actual call.</span></span>

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
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
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
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


