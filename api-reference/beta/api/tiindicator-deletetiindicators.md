---
title: 'tiIndicator: deleteTiIndicators'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9e11defaf3d505d5566c9d5d720e26b6c88447a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022203"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="639df-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="639df-103">tiIndicator: deleteTiIndicators</span></span>

<span data-ttu-id="639df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="639df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="639df-105">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="639df-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="639df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="639df-106">Permissions</span></span>

<span data-ttu-id="639df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="639df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="639df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="639df-109">Permission type</span></span> | <span data-ttu-id="639df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="639df-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="639df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="639df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="639df-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="639df-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="639df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="639df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="639df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="639df-114">Not supported.</span></span> |
| <span data-ttu-id="639df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="639df-115">Application</span></span>                            | <span data-ttu-id="639df-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="639df-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="639df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="639df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="639df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="639df-118">Request headers</span></span>

| <span data-ttu-id="639df-119">Nome</span><span class="sxs-lookup"><span data-stu-id="639df-119">Name</span></span>          | <span data-ttu-id="639df-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="639df-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="639df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="639df-121">Authorization</span></span> | <span data-ttu-id="639df-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="639df-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="639df-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="639df-123">Request body</span></span>

<span data-ttu-id="639df-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="639df-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="639df-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="639df-125">Parameter</span></span>    | <span data-ttu-id="639df-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="639df-126">Type</span></span>        | <span data-ttu-id="639df-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="639df-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="639df-128">valor</span><span class="sxs-lookup"><span data-stu-id="639df-128">value</span></span>|<span data-ttu-id="639df-129">Coleção String</span><span class="sxs-lookup"><span data-stu-id="639df-129">String collection</span></span>| <span data-ttu-id="639df-130">Coleção de tiIndicator `id` s a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="639df-130">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="639df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="639df-131">Response</span></span>

<span data-ttu-id="639df-132">Se bem-sucedido, este método retorna o `200, OK` código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="639df-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="639df-133">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="639df-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="639df-134">Consulte [erros](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="639df-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="639df-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="639df-135">Examples</span></span>

<span data-ttu-id="639df-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="639df-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="639df-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="639df-137">Request</span></span>

<span data-ttu-id="639df-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="639df-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="639df-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="639df-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="639df-140">C#</span><span class="sxs-lookup"><span data-stu-id="639df-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="639df-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="639df-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="639df-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="639df-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="639df-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="639df-143">Response</span></span>

<span data-ttu-id="639df-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="639df-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="639df-145">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="639df-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="639df-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="639df-146">All the properties will be returned from an actual call.</span></span>

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


