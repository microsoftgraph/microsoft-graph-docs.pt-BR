---
title: 'tiIndicator: updateTiIndicators'
description: Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: fa2cc1375a76ab1ccf0f5be86c46c6fc26d50578
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409279"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="95ce6-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="95ce6-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95ce6-104">Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="95ce6-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="95ce6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="95ce6-105">Permissions</span></span>

<span data-ttu-id="95ce6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95ce6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95ce6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95ce6-108">Permission type</span></span>   | <span data-ttu-id="95ce6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95ce6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="95ce6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95ce6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="95ce6-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="95ce6-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="95ce6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95ce6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95ce6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95ce6-113">Not supported.</span></span> |
| <span data-ttu-id="95ce6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95ce6-114">Application</span></span>                            | <span data-ttu-id="95ce6-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="95ce6-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="95ce6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95ce6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="95ce6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95ce6-117">Request headers</span></span>

| <span data-ttu-id="95ce6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="95ce6-118">Name</span></span>          | <span data-ttu-id="95ce6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="95ce6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="95ce6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="95ce6-120">Authorization</span></span> | <span data-ttu-id="95ce6-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="95ce6-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="95ce6-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95ce6-122">Request body</span></span>

<span data-ttu-id="95ce6-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95ce6-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="95ce6-124">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update tiIndicator](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="95ce6-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="95ce6-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="95ce6-125">Parameter</span></span>    | <span data-ttu-id="95ce6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="95ce6-126">Type</span></span>        | <span data-ttu-id="95ce6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="95ce6-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95ce6-128">valor</span><span class="sxs-lookup"><span data-stu-id="95ce6-128">value</span></span>|<span data-ttu-id="95ce6-129">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="95ce6-129">tiIndicator collection</span></span>| <span data-ttu-id="95ce6-130">Coleção de **tiIndicators** para atualizar.</span><span class="sxs-lookup"><span data-stu-id="95ce6-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="95ce6-131">Cada entidade deve ter **ID** e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="95ce6-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="95ce6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="95ce6-132">Response</span></span>

<span data-ttu-id="95ce6-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95ce6-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95ce6-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95ce6-134">Examples</span></span>

<span data-ttu-id="95ce6-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="95ce6-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="95ce6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95ce6-136">Request</span></span>

<span data-ttu-id="95ce6-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="95ce6-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95ce6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="95ce6-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="95ce6-139">C#</span><span class="sxs-lookup"><span data-stu-id="95ce6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95ce6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95ce6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95ce6-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="95ce6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95ce6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="95ce6-142">Response</span></span>

<span data-ttu-id="95ce6-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95ce6-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="95ce6-144">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="95ce6-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95ce6-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95ce6-145">All the properties will be returned from an actual call.</span></span>

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
