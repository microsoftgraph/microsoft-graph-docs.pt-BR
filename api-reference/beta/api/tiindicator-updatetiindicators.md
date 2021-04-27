---
title: 'tiIndicator: updateTiIndicators'
description: Atualize vários indicadores de TI (inteligência contra ameaças) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4c594c9ba75ea0ee1cd1fcb8390d4b9ff738d48c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050770"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="964a5-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="964a5-103">tiIndicator: updateTiIndicators</span></span>

<span data-ttu-id="964a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="964a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="964a5-105">Atualize vários indicadores de TI (inteligência contra ameaças) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="964a5-105">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="964a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="964a5-106">Permissions</span></span>

<span data-ttu-id="964a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="964a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="964a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="964a5-109">Permission type</span></span>   | <span data-ttu-id="964a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="964a5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="964a5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="964a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="964a5-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="964a5-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="964a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="964a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="964a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="964a5-114">Not supported.</span></span> |
| <span data-ttu-id="964a5-115">Application</span><span class="sxs-lookup"><span data-stu-id="964a5-115">Application</span></span>                            | <span data-ttu-id="964a5-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="964a5-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="964a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="964a5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="964a5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="964a5-118">Request headers</span></span>

| <span data-ttu-id="964a5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="964a5-119">Name</span></span>          | <span data-ttu-id="964a5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="964a5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="964a5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="964a5-121">Authorization</span></span> | <span data-ttu-id="964a5-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="964a5-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="964a5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="964a5-123">Request body</span></span>

<span data-ttu-id="964a5-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="964a5-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="964a5-125">Para obter detalhes sobre propriedades que podem ser atualizadas, consulte [update tiIndicator](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="964a5-125">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="964a5-126">Os campos necessários para cada tiIndicator são: `id` , `expirationDateTime` , `targetProduct` .</span><span class="sxs-lookup"><span data-stu-id="964a5-126">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="964a5-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="964a5-127">Parameter</span></span>    | <span data-ttu-id="964a5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="964a5-128">Type</span></span>        | <span data-ttu-id="964a5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="964a5-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="964a5-130">valor</span><span class="sxs-lookup"><span data-stu-id="964a5-130">value</span></span>|<span data-ttu-id="964a5-131">Coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="964a5-131">tiIndicator collection</span></span>| <span data-ttu-id="964a5-132">Coleção **de tiIndicators** a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="964a5-132">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="964a5-133">Cada entidade deve ter **id** e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="964a5-133">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="964a5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="964a5-134">Response</span></span>

<span data-ttu-id="964a5-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="964a5-135">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="964a5-136">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="964a5-136">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="964a5-137">Consulte [Erros para](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="964a5-137">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="964a5-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="964a5-138">Examples</span></span>

<span data-ttu-id="964a5-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="964a5-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="964a5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="964a5-140">Request</span></span>

<span data-ttu-id="964a5-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="964a5-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="964a5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="964a5-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="964a5-143">C#</span><span class="sxs-lookup"><span data-stu-id="964a5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="964a5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="964a5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="964a5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="964a5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="964a5-146">Java</span><span class="sxs-lookup"><span data-stu-id="964a5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-updatetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="964a5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="964a5-147">Response</span></span>

<span data-ttu-id="964a5-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="964a5-148">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="964a5-149">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="964a5-149">The response object shown here might be shortened for readability.</span></span>

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


