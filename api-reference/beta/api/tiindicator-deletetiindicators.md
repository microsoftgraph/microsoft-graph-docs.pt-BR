---
title: 'tiIndicator: deleteTiIndicators'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3941ba24ab46006790e2682cd6e345a5b89217ba
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453345"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="52aef-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="52aef-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52aef-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="52aef-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="52aef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52aef-105">Permissions</span></span>

<span data-ttu-id="52aef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52aef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52aef-108">Permission type</span></span> | <span data-ttu-id="52aef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52aef-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52aef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52aef-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="52aef-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="52aef-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="52aef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52aef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52aef-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52aef-113">Not supported.</span></span> |
| <span data-ttu-id="52aef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52aef-114">Application</span></span>                            | <span data-ttu-id="52aef-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="52aef-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="52aef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52aef-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="52aef-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52aef-117">Request headers</span></span>

| <span data-ttu-id="52aef-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52aef-118">Name</span></span>          | <span data-ttu-id="52aef-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="52aef-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="52aef-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52aef-120">Authorization</span></span> | <span data-ttu-id="52aef-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="52aef-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="52aef-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52aef-122">Request body</span></span>

<span data-ttu-id="52aef-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52aef-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52aef-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52aef-124">Parameter</span></span>    | <span data-ttu-id="52aef-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="52aef-125">Type</span></span>        | <span data-ttu-id="52aef-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="52aef-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52aef-127">valor</span><span class="sxs-lookup"><span data-stu-id="52aef-127">value</span></span>|<span data-ttu-id="52aef-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="52aef-128">String collection</span></span>| <span data-ttu-id="52aef-129">Coleção de tiIndicator `id`s a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="52aef-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="52aef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52aef-130">Response</span></span>

<span data-ttu-id="52aef-131">Se bem-sucedido, este método retorna `200, OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52aef-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52aef-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52aef-132">Examples</span></span>

<span data-ttu-id="52aef-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="52aef-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="52aef-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52aef-134">Request</span></span>

<span data-ttu-id="52aef-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52aef-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52aef-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="52aef-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="52aef-137">C#</span><span class="sxs-lookup"><span data-stu-id="52aef-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52aef-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="52aef-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52aef-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52aef-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52aef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="52aef-140">Response</span></span>

<span data-ttu-id="52aef-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52aef-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="52aef-142">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52aef-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52aef-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52aef-143">All the properties will be returned from an actual call.</span></span>

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
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
