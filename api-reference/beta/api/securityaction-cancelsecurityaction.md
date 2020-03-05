---
title: 'SecurityAction: cancelSecurityAction'
description: Cancela uma operação de segurança.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 5f9800c5f5755721758c7db552aab7ac150a263f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453587"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="dcf33-103">SecurityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="dcf33-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="dcf33-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dcf33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf33-105">Cancela uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="dcf33-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcf33-106">Permissions</span></span>

<span data-ttu-id="dcf33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcf33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcf33-109">Permission type</span></span>                        | <span data-ttu-id="dcf33-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcf33-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcf33-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcf33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcf33-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcf33-112">Not supported.</span></span> |
| <span data-ttu-id="dcf33-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcf33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcf33-114">Not supported.</span></span> |
| <span data-ttu-id="dcf33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcf33-115">Application</span></span>                            | <span data-ttu-id="dcf33-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcf33-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf33-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="dcf33-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf33-118">Request headers</span></span>

| <span data-ttu-id="dcf33-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dcf33-119">Name</span></span>          | <span data-ttu-id="dcf33-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcf33-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dcf33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf33-121">Authorization</span></span> | <span data-ttu-id="dcf33-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="dcf33-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf33-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf33-123">Request body</span></span>

<span data-ttu-id="dcf33-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcf33-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf33-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf33-125">Response</span></span>

<span data-ttu-id="dcf33-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcf33-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcf33-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcf33-128">Examples</span></span>

<span data-ttu-id="dcf33-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="dcf33-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dcf33-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf33-130">Request</span></span>

<span data-ttu-id="dcf33-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcf33-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcf33-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf33-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="dcf33-133">C#</span><span class="sxs-lookup"><span data-stu-id="dcf33-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcf33-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcf33-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcf33-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcf33-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcf33-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf33-136">Response</span></span>

<span data-ttu-id="dcf33-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcf33-137">The following is an example of the response.</span></span>
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
