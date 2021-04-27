---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: Exclua vários indicadores de TI (inteligência de ameaça) em uma solicitação em vez de várias solicitações, e a solicitação contém IDs externas em vez de IDs.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a163f2c2a362cda42964733bf6639a2138dcb98c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052660"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="20922-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="20922-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

<span data-ttu-id="20922-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20922-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20922-105">Exclua vários indicadores de TI (inteligência de ameaça) em uma solicitação em vez de várias solicitações, quando a solicitação contiver IDs externas em vez de IDs.</span><span class="sxs-lookup"><span data-stu-id="20922-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="20922-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20922-106">Permissions</span></span>

<span data-ttu-id="20922-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20922-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20922-109">Permission type</span></span>  | <span data-ttu-id="20922-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20922-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20922-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20922-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20922-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="20922-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="20922-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20922-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20922-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20922-114">Not supported.</span></span> |
| <span data-ttu-id="20922-115">Application</span><span class="sxs-lookup"><span data-stu-id="20922-115">Application</span></span>                            | <span data-ttu-id="20922-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="20922-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="20922-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20922-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="20922-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20922-118">Request headers</span></span>

| <span data-ttu-id="20922-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20922-119">Name</span></span>          | <span data-ttu-id="20922-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20922-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="20922-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20922-121">Authorization</span></span> | <span data-ttu-id="20922-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="20922-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="20922-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20922-123">Request body</span></span>

<span data-ttu-id="20922-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20922-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20922-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20922-125">Parameter</span></span>    | <span data-ttu-id="20922-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="20922-126">Type</span></span>        | <span data-ttu-id="20922-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="20922-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20922-128">valor</span><span class="sxs-lookup"><span data-stu-id="20922-128">value</span></span>|<span data-ttu-id="20922-129">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="20922-129">String collection</span></span>| <span data-ttu-id="20922-130">Coleção dos `externalIds` **objetos tiIndicator** a serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="20922-130">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="20922-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="20922-131">Response</span></span>

<span data-ttu-id="20922-132">Se tiver êxito, este método retornará `200, OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20922-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="20922-133">Se houver um erro, este método retornará um `206 Partial Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="20922-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="20922-134">Consulte [Erros para](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="20922-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="20922-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20922-135">Examples</span></span>

<span data-ttu-id="20922-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="20922-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="20922-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20922-137">Request</span></span>

<span data-ttu-id="20922-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20922-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20922-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="20922-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="20922-140">C#</span><span class="sxs-lookup"><span data-stu-id="20922-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicatorsbyexternalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20922-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20922-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicatorsbyexternalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20922-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20922-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicatorsbyexternalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20922-143">Java</span><span class="sxs-lookup"><span data-stu-id="20922-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicatorsbyexternalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20922-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20922-144">Response</span></span>

<span data-ttu-id="20922-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20922-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="20922-146">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="20922-146">The response object shown here might be shortened for readability.</span></span>

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
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


