---
title: 'tiIndicator: deleteTiIndicators'
description: Exclua vários indicadores de TI (inteligência contra ameaças) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 365f4c803cb7f6e7b18570534819e576990d11de
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050791"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="3123c-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="3123c-103">tiIndicator: deleteTiIndicators</span></span>

<span data-ttu-id="3123c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3123c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3123c-105">Exclua vários indicadores de TI (inteligência contra ameaças) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="3123c-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="3123c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3123c-106">Permissions</span></span>

<span data-ttu-id="3123c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3123c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3123c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3123c-109">Permission type</span></span> | <span data-ttu-id="3123c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3123c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3123c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3123c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3123c-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3123c-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="3123c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3123c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3123c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3123c-114">Not supported.</span></span> |
| <span data-ttu-id="3123c-115">Application</span><span class="sxs-lookup"><span data-stu-id="3123c-115">Application</span></span>                            | <span data-ttu-id="3123c-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3123c-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="3123c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3123c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="3123c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3123c-118">Request headers</span></span>

| <span data-ttu-id="3123c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3123c-119">Name</span></span>          | <span data-ttu-id="3123c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3123c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3123c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3123c-121">Authorization</span></span> | <span data-ttu-id="3123c-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3123c-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3123c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3123c-123">Request body</span></span>

<span data-ttu-id="3123c-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3123c-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3123c-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3123c-125">Parameter</span></span>    | <span data-ttu-id="3123c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3123c-126">Type</span></span>        | <span data-ttu-id="3123c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3123c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3123c-128">valor</span><span class="sxs-lookup"><span data-stu-id="3123c-128">value</span></span>|<span data-ttu-id="3123c-129">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3123c-129">String collection</span></span>| <span data-ttu-id="3123c-130">Coleção de tiIndicator `id` s a serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="3123c-130">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="3123c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3123c-131">Response</span></span>

<span data-ttu-id="3123c-132">Se tiver êxito, este método retornará `200, OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3123c-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="3123c-133">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="3123c-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="3123c-134">Consulte [Erros para](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="3123c-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="3123c-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3123c-135">Examples</span></span>

<span data-ttu-id="3123c-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3123c-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3123c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3123c-137">Request</span></span>

<span data-ttu-id="3123c-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3123c-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3123c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3123c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="3123c-140">C#</span><span class="sxs-lookup"><span data-stu-id="3123c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3123c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3123c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3123c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3123c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3123c-143">Java</span><span class="sxs-lookup"><span data-stu-id="3123c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3123c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3123c-144">Response</span></span>

<span data-ttu-id="3123c-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3123c-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3123c-146">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="3123c-146">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": 0,
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


