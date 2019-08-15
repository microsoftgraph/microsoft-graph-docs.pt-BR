---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação, em vez de várias solicitações, e a solicitação contém IDs externas em vez de IDs.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 897bc28bb372f76522a0bfc30dd521610ce7f6a5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421257"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="a4b60-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="a4b60-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4b60-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação, em vez de várias solicitações, quando a solicitação contém IDs externas em vez de IDs.</span><span class="sxs-lookup"><span data-stu-id="a4b60-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4b60-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4b60-105">Permissions</span></span>

<span data-ttu-id="a4b60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4b60-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4b60-108">Permission type</span></span>  | <span data-ttu-id="a4b60-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4b60-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a4b60-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4b60-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4b60-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a4b60-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="a4b60-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4b60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4b60-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4b60-113">Not supported.</span></span> |
| <span data-ttu-id="a4b60-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4b60-114">Application</span></span>                            | <span data-ttu-id="a4b60-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a4b60-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4b60-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4b60-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="a4b60-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b60-117">Request headers</span></span>

| <span data-ttu-id="a4b60-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a4b60-118">Name</span></span>          | <span data-ttu-id="a4b60-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4b60-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a4b60-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4b60-120">Authorization</span></span> | <span data-ttu-id="a4b60-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a4b60-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4b60-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b60-122">Request body</span></span>

<span data-ttu-id="a4b60-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4b60-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4b60-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4b60-124">Parameter</span></span>    | <span data-ttu-id="a4b60-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4b60-125">Type</span></span>        | <span data-ttu-id="a4b60-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4b60-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4b60-127">valor</span><span class="sxs-lookup"><span data-stu-id="a4b60-127">value</span></span>|<span data-ttu-id="a4b60-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4b60-128">String collection</span></span>| <span data-ttu-id="a4b60-129">Coleção de `externalIds` objetos **tiIndicator** a serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="a4b60-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="a4b60-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4b60-130">Response</span></span>

<span data-ttu-id="a4b60-131">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4b60-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4b60-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4b60-132">Examples</span></span>

<span data-ttu-id="a4b60-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a4b60-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a4b60-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b60-134">Request</span></span>

<span data-ttu-id="a4b60-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4b60-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4b60-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4b60-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4b60-137">C#</span><span class="sxs-lookup"><span data-stu-id="a4b60-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicatorsbyexternalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4b60-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4b60-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicatorsbyexternalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4b60-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a4b60-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicatorsbyexternalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4b60-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4b60-140">Response</span></span>

<span data-ttu-id="a4b60-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4b60-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a4b60-142">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4b60-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a4b60-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4b60-143">All the properties will be returned from an actual call.</span></span>

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
      "code": "code-value",
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
