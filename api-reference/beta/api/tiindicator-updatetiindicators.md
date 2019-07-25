---
title: 'tiIndicator: updateTiIndicators'
description: Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b50699925efab2d5baf3f67d9937ee281c88d2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868143"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="21bf3-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="21bf3-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21bf3-104">Atualize vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="21bf3-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="21bf3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="21bf3-105">Permissions</span></span>

<span data-ttu-id="21bf3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21bf3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21bf3-108">Permission type</span></span>   | <span data-ttu-id="21bf3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21bf3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="21bf3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21bf3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="21bf3-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="21bf3-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="21bf3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21bf3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21bf3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21bf3-113">Not supported.</span></span> |
| <span data-ttu-id="21bf3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21bf3-114">Application</span></span>                            | <span data-ttu-id="21bf3-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="21bf3-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="21bf3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21bf3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="21bf3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21bf3-117">Request headers</span></span>

| <span data-ttu-id="21bf3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="21bf3-118">Name</span></span>          | <span data-ttu-id="21bf3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="21bf3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="21bf3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="21bf3-120">Authorization</span></span> | <span data-ttu-id="21bf3-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="21bf3-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="21bf3-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21bf3-122">Request body</span></span>

<span data-ttu-id="21bf3-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21bf3-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="21bf3-124">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update tiIndicator](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="21bf3-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="21bf3-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="21bf3-125">Parameter</span></span>    | <span data-ttu-id="21bf3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="21bf3-126">Type</span></span>        | <span data-ttu-id="21bf3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="21bf3-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21bf3-128">valor</span><span class="sxs-lookup"><span data-stu-id="21bf3-128">value</span></span>|<span data-ttu-id="21bf3-129">coleção tiIndicator</span><span class="sxs-lookup"><span data-stu-id="21bf3-129">tiIndicator collection</span></span>| <span data-ttu-id="21bf3-130">Coleção de **tiIndicators** para atualizar.</span><span class="sxs-lookup"><span data-stu-id="21bf3-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="21bf3-131">Cada entidade deve ter **ID** e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="21bf3-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="21bf3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="21bf3-132">Response</span></span>

<span data-ttu-id="21bf3-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21bf3-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21bf3-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="21bf3-134">Examples</span></span>

<span data-ttu-id="21bf3-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="21bf3-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="21bf3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21bf3-136">Request</span></span>

<span data-ttu-id="21bf3-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21bf3-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21bf3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="21bf3-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="21bf3-139">C#</span><span class="sxs-lookup"><span data-stu-id="21bf3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21bf3-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="21bf3-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21bf3-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="21bf3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21bf3-142">Java</span><span class="sxs-lookup"><span data-stu-id="21bf3-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-updatetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21bf3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="21bf3-143">Response</span></span>

<span data-ttu-id="21bf3-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21bf3-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="21bf3-145">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21bf3-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21bf3-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21bf3-146">All the properties will be returned from an actual call.</span></span>

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
