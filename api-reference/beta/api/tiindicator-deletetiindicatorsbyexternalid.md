---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação, em vez de várias solicitações, e a solicitação contém IDs externas em vez de IDs.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: cdc1f1f6bb0d467afd86c653d147cf3c7bed8a62
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987919"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="19b42-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="19b42-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19b42-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação, em vez de várias solicitações, quando a solicitação contém IDs externas em vez de IDs.</span><span class="sxs-lookup"><span data-stu-id="19b42-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="19b42-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="19b42-105">Permissions</span></span>

<span data-ttu-id="19b42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19b42-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19b42-108">Permission type</span></span>  | <span data-ttu-id="19b42-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19b42-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19b42-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19b42-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19b42-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="19b42-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="19b42-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19b42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19b42-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19b42-113">Not supported.</span></span> |
| <span data-ttu-id="19b42-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19b42-114">Application</span></span>                            | <span data-ttu-id="19b42-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="19b42-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="19b42-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19b42-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="19b42-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19b42-117">Request headers</span></span>

| <span data-ttu-id="19b42-118">Nome</span><span class="sxs-lookup"><span data-stu-id="19b42-118">Name</span></span>          | <span data-ttu-id="19b42-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b42-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19b42-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="19b42-120">Authorization</span></span> | <span data-ttu-id="19b42-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="19b42-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="19b42-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19b42-122">Request body</span></span>

<span data-ttu-id="19b42-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19b42-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19b42-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19b42-124">Parameter</span></span>    | <span data-ttu-id="19b42-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="19b42-125">Type</span></span>        | <span data-ttu-id="19b42-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b42-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19b42-127">valor</span><span class="sxs-lookup"><span data-stu-id="19b42-127">value</span></span>|<span data-ttu-id="19b42-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="19b42-128">String collection</span></span>| <span data-ttu-id="19b42-129">Coleção de `externalIds` objetos **tiIndicator** a serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="19b42-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="19b42-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b42-130">Response</span></span>

<span data-ttu-id="19b42-131">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19b42-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19b42-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19b42-132">Examples</span></span>

<span data-ttu-id="19b42-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="19b42-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="19b42-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19b42-134">Request</span></span>

<span data-ttu-id="19b42-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19b42-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19b42-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="19b42-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="19b42-137">C#</span><span class="sxs-lookup"><span data-stu-id="19b42-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicatorsbyexternalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19b42-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="19b42-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicatorsbyexternalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19b42-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="19b42-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicatorsbyexternalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19b42-140">Java</span><span class="sxs-lookup"><span data-stu-id="19b42-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicatorsbyexternalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19b42-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b42-141">Response</span></span>

<span data-ttu-id="19b42-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19b42-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="19b42-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19b42-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="19b42-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19b42-144">All the properties will be returned from an actual call.</span></span>

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
