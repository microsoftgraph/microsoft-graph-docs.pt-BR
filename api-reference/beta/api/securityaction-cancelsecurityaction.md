---
title: 'SecurityAction: cancelSecurityAction'
description: Cancela uma operação de segurança.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 138f4b8bd30b453ce98e4c5c036e28d19a15b094
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266945"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="71e0c-103">SecurityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="71e0c-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71e0c-104">Cancela uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="71e0c-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="71e0c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="71e0c-105">Permissions</span></span>

<span data-ttu-id="71e0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71e0c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71e0c-108">Permission type</span></span>                        | <span data-ttu-id="71e0c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71e0c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71e0c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71e0c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="71e0c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71e0c-111">Not supported.</span></span> |
| <span data-ttu-id="71e0c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71e0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71e0c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71e0c-113">Not supported.</span></span> |
| <span data-ttu-id="71e0c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71e0c-114">Application</span></span>                            | <span data-ttu-id="71e0c-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71e0c-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71e0c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71e0c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="71e0c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71e0c-117">Request headers</span></span>

| <span data-ttu-id="71e0c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="71e0c-118">Name</span></span>          | <span data-ttu-id="71e0c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="71e0c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="71e0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71e0c-120">Authorization</span></span> | <span data-ttu-id="71e0c-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="71e0c-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="71e0c-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71e0c-122">Request body</span></span>

<span data-ttu-id="71e0c-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71e0c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71e0c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="71e0c-124">Response</span></span>

<span data-ttu-id="71e0c-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71e0c-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71e0c-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71e0c-127">Examples</span></span>

<span data-ttu-id="71e0c-128">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="71e0c-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="71e0c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71e0c-129">Request</span></span>

<span data-ttu-id="71e0c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71e0c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="71e0c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="71e0c-131">Response</span></span>

<span data-ttu-id="71e0c-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71e0c-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="71e0c-133">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="71e0c-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="71e0c-134">C#</span><span class="sxs-lookup"><span data-stu-id="71e0c-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71e0c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="71e0c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="71e0c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="71e0c-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
