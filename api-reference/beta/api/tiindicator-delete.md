---
title: Excluir indicador de inteligência de ameaças
description: Excluir um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: aa7ceefca5201930f97d5e7befb6a7cc43c5715a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637595"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="656d4-103">Excluir indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="656d4-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="656d4-104">Excluir um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="656d4-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="656d4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="656d4-105">Permissions</span></span>

<span data-ttu-id="656d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="656d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="656d4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="656d4-108">Permission type</span></span>                        | <span data-ttu-id="656d4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="656d4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="656d4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="656d4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="656d4-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="656d4-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="656d4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="656d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="656d4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="656d4-113">Not supported.</span></span> |
| <span data-ttu-id="656d4-114">Application</span><span class="sxs-lookup"><span data-stu-id="656d4-114">Application</span></span>                            | <span data-ttu-id="656d4-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="656d4-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="656d4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="656d4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="656d4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="656d4-117">Request headers</span></span>

| <span data-ttu-id="656d4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="656d4-118">Name</span></span>          | <span data-ttu-id="656d4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="656d4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="656d4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="656d4-120">Authorization</span></span> | <span data-ttu-id="656d4-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="656d4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="656d4-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="656d4-122">Request body</span></span>

<span data-ttu-id="656d4-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="656d4-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="656d4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="656d4-124">Response</span></span>

<span data-ttu-id="656d4-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="656d4-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="656d4-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="656d4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="656d4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="656d4-128">Request</span></span>

<span data-ttu-id="656d4-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="656d4-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="656d4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="656d4-130">Response</span></span>

<span data-ttu-id="656d4-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="656d4-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="656d4-132">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="656d4-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="656d4-133">Basic</span><span class="sxs-lookup"><span data-stu-id="656d4-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="656d4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="656d4-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
