---
title: 'tiIndicator: deleteTiIndicators'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d8925c4e998558f9adf5d96c742dbedafc93d4ae
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270697"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="bbf9b-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="bbf9b-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf9b-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbf9b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbf9b-105">Permissions</span></span>

<span data-ttu-id="bbf9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbf9b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf9b-108">Permission type</span></span> | <span data-ttu-id="bbf9b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbf9b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bbf9b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf9b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbf9b-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="bbf9b-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="bbf9b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf9b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-113">Not supported.</span></span> |
| <span data-ttu-id="bbf9b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf9b-114">Application</span></span>                            | <span data-ttu-id="bbf9b-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="bbf9b-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbf9b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf9b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="bbf9b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf9b-117">Request headers</span></span>

| <span data-ttu-id="bbf9b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bbf9b-118">Name</span></span>          | <span data-ttu-id="bbf9b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf9b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bbf9b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbf9b-120">Authorization</span></span> | <span data-ttu-id="bbf9b-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bbf9b-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbf9b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf9b-122">Request body</span></span>

<span data-ttu-id="bbf9b-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbf9b-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbf9b-124">Parameter</span></span>    | <span data-ttu-id="bbf9b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbf9b-125">Type</span></span>        | <span data-ttu-id="bbf9b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf9b-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbf9b-127">valor</span><span class="sxs-lookup"><span data-stu-id="bbf9b-127">value</span></span>|<span data-ttu-id="bbf9b-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf9b-128">String collection</span></span>| <span data-ttu-id="bbf9b-129">Coleção de tiIndicator `id`s a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="bbf9b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf9b-130">Response</span></span>

<span data-ttu-id="bbf9b-131">Se bem-sucedido, este método retorna `200, OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbf9b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bbf9b-132">Examples</span></span>

<span data-ttu-id="bbf9b-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bbf9b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf9b-134">Request</span></span>

<span data-ttu-id="bbf9b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bbf9b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf9b-136">Response</span></span>

<span data-ttu-id="bbf9b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bbf9b-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bbf9b-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-139">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bbf9b-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bbf9b-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bbf9b-141">C#</span><span class="sxs-lookup"><span data-stu-id="bbf9b-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbf9b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbf9b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bbf9b-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bbf9b-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
