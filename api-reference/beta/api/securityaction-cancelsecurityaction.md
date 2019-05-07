---
title: 'SecurityAction: cancelSecurityAction'
description: Cancela uma operação de segurança.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 33fa78176dcb32bad889c7d3336177ef96aaa0b6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638904"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="b2d07-103">SecurityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="b2d07-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d07-104">Cancela uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="b2d07-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2d07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2d07-105">Permissions</span></span>

<span data-ttu-id="b2d07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2d07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2d07-108">Permission type</span></span>                        | <span data-ttu-id="b2d07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2d07-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2d07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2d07-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2d07-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d07-111">Not supported.</span></span> |
| <span data-ttu-id="b2d07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2d07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2d07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d07-113">Not supported.</span></span> |
| <span data-ttu-id="b2d07-114">Application</span><span class="sxs-lookup"><span data-stu-id="b2d07-114">Application</span></span>                            | <span data-ttu-id="b2d07-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d07-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2d07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d07-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="b2d07-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d07-117">Request headers</span></span>

| <span data-ttu-id="b2d07-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b2d07-118">Name</span></span>          | <span data-ttu-id="b2d07-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d07-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b2d07-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2d07-120">Authorization</span></span> | <span data-ttu-id="b2d07-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b2d07-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2d07-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d07-122">Request body</span></span>

<span data-ttu-id="b2d07-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2d07-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2d07-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d07-124">Response</span></span>

<span data-ttu-id="b2d07-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d07-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2d07-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b2d07-127">Examples</span></span>

<span data-ttu-id="b2d07-128">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b2d07-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b2d07-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d07-129">Request</span></span>

<span data-ttu-id="b2d07-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d07-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="b2d07-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d07-131">Response</span></span>

<span data-ttu-id="b2d07-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d07-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2d07-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b2d07-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b2d07-134">Basic</span><span class="sxs-lookup"><span data-stu-id="b2d07-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2d07-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2d07-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
