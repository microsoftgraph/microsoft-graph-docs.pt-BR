---
title: Excluir indicador de inteligência de ameaças
description: Excluir um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e7a1f3af86ec603c360d66d1b3c9d757d1da2254
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270725"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="cb3ff-103">Excluir indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="cb3ff-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb3ff-104">Excluir um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="cb3ff-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb3ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb3ff-105">Permissions</span></span>

<span data-ttu-id="cb3ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb3ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb3ff-108">Permission type</span></span>                        | <span data-ttu-id="cb3ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb3ff-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb3ff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb3ff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb3ff-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cb3ff-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="cb3ff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb3ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb3ff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb3ff-113">Not supported.</span></span> |
| <span data-ttu-id="cb3ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb3ff-114">Application</span></span>                            | <span data-ttu-id="cb3ff-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cb3ff-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb3ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb3ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb3ff-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3ff-117">Request headers</span></span>

| <span data-ttu-id="cb3ff-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cb3ff-118">Name</span></span>          | <span data-ttu-id="cb3ff-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb3ff-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cb3ff-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3ff-120">Authorization</span></span> | <span data-ttu-id="cb3ff-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cb3ff-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb3ff-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3ff-122">Request body</span></span>

<span data-ttu-id="cb3ff-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb3ff-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb3ff-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb3ff-124">Response</span></span>

<span data-ttu-id="cb3ff-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb3ff-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb3ff-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb3ff-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb3ff-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3ff-128">Request</span></span>

<span data-ttu-id="cb3ff-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb3ff-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="cb3ff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb3ff-130">Response</span></span>

<span data-ttu-id="cb3ff-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb3ff-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cb3ff-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="cb3ff-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cb3ff-133">C#</span><span class="sxs-lookup"><span data-stu-id="cb3ff-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb3ff-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb3ff-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cb3ff-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cb3ff-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
