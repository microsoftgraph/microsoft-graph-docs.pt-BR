---
title: 'SecurityAction: cancelSecurityAction'
description: Cancela uma operação de segurança.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 2f3e029bcbf417678b94cea00934eb993672cb71
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410385"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="02554-103">SecurityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="02554-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02554-104">Cancela uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="02554-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="02554-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02554-105">Permissions</span></span>

<span data-ttu-id="02554-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02554-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02554-108">Permission type</span></span>                        | <span data-ttu-id="02554-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02554-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02554-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02554-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02554-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02554-111">Not supported.</span></span> |
| <span data-ttu-id="02554-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02554-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02554-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02554-113">Not supported.</span></span> |
| <span data-ttu-id="02554-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02554-114">Application</span></span>                            | <span data-ttu-id="02554-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02554-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02554-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02554-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="02554-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02554-117">Request headers</span></span>

| <span data-ttu-id="02554-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02554-118">Name</span></span>          | <span data-ttu-id="02554-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02554-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="02554-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="02554-120">Authorization</span></span> | <span data-ttu-id="02554-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="02554-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="02554-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02554-122">Request body</span></span>

<span data-ttu-id="02554-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02554-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02554-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="02554-124">Response</span></span>

<span data-ttu-id="02554-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02554-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02554-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02554-127">Examples</span></span>

<span data-ttu-id="02554-128">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="02554-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="02554-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02554-129">Request</span></span>

<span data-ttu-id="02554-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02554-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02554-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="02554-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02554-132">C#</span><span class="sxs-lookup"><span data-stu-id="02554-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02554-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02554-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02554-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="02554-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02554-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="02554-135">Response</span></span>

<span data-ttu-id="02554-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02554-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
