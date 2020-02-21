---
title: 'tiIndicator: updateTiIndicators'
description: Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 6c844f77c33ad69b322b7ab5120a76580c991d0e
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219717"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="52a56-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="52a56-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a56-104">Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="52a56-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="52a56-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52a56-105">Permissions</span></span>

<span data-ttu-id="52a56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52a56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52a56-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52a56-108">Permission type</span></span>   | <span data-ttu-id="52a56-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52a56-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52a56-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52a56-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="52a56-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="52a56-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="52a56-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52a56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52a56-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52a56-113">Not supported.</span></span> |
| <span data-ttu-id="52a56-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52a56-114">Application</span></span>                            | <span data-ttu-id="52a56-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="52a56-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="52a56-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52a56-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="52a56-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52a56-117">Request headers</span></span>

| <span data-ttu-id="52a56-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52a56-118">Name</span></span>          | <span data-ttu-id="52a56-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a56-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="52a56-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52a56-120">Authorization</span></span> | <span data-ttu-id="52a56-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="52a56-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="52a56-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52a56-122">Request body</span></span>

<span data-ttu-id="52a56-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52a56-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="52a56-124">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update tiIndicator](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="52a56-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="52a56-125">Os campos obrigatórios para cada tiIndicator `id`são `expirationDateTime`: `targetProduct`,,.</span><span class="sxs-lookup"><span data-stu-id="52a56-125">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="52a56-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52a56-126">Parameter</span></span>    | <span data-ttu-id="52a56-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="52a56-127">Type</span></span>        | <span data-ttu-id="52a56-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a56-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52a56-129">valor</span><span class="sxs-lookup"><span data-stu-id="52a56-129">value</span></span>|<span data-ttu-id="52a56-130">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="52a56-130">tiIndicator collection</span></span>| <span data-ttu-id="52a56-131">Coleção de **tiIndicators** para atualizar.</span><span class="sxs-lookup"><span data-stu-id="52a56-131">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="52a56-132">Cada entidade deve ter **ID** e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="52a56-132">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="52a56-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="52a56-133">Response</span></span>

<span data-ttu-id="52a56-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52a56-134">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="52a56-135">Se houver um erro, este método retornará um código `206 Partial Content` de resposta.</span><span class="sxs-lookup"><span data-stu-id="52a56-135">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="52a56-136">Consulte [erros](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="52a56-136">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="52a56-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52a56-137">Examples</span></span>

<span data-ttu-id="52a56-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="52a56-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="52a56-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52a56-139">Request</span></span>

<span data-ttu-id="52a56-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52a56-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52a56-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="52a56-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="52a56-142">C#</span><span class="sxs-lookup"><span data-stu-id="52a56-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52a56-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52a56-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52a56-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52a56-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52a56-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="52a56-145">Response</span></span>

<span data-ttu-id="52a56-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52a56-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="52a56-147">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52a56-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52a56-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52a56-148">All the properties will be returned from an actual call.</span></span>

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
