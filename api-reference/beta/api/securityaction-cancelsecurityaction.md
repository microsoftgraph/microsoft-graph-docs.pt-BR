---
title: 'SecurityAction: cancelSecurityAction'
description: Cancela uma operação de segurança.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 87cb0eca08e1d8c1dce81440fbaed40d12b46fa8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046936"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="cea40-103">SecurityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="cea40-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="cea40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cea40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cea40-105">Cancela uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="cea40-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="cea40-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cea40-106">Permissions</span></span>

<span data-ttu-id="cea40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cea40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cea40-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cea40-109">Permission type</span></span>                        | <span data-ttu-id="cea40-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cea40-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cea40-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cea40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cea40-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cea40-112">Not supported.</span></span> |
| <span data-ttu-id="cea40-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cea40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cea40-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cea40-114">Not supported.</span></span> |
| <span data-ttu-id="cea40-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cea40-115">Application</span></span>                            | <span data-ttu-id="cea40-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cea40-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cea40-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cea40-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="cea40-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cea40-118">Request headers</span></span>

| <span data-ttu-id="cea40-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cea40-119">Name</span></span>          | <span data-ttu-id="cea40-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cea40-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cea40-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cea40-121">Authorization</span></span> | <span data-ttu-id="cea40-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cea40-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cea40-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cea40-123">Request body</span></span>

<span data-ttu-id="cea40-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cea40-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cea40-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="cea40-125">Response</span></span>

<span data-ttu-id="cea40-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cea40-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cea40-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cea40-128">Examples</span></span>

<span data-ttu-id="cea40-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cea40-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cea40-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cea40-130">Request</span></span>

<span data-ttu-id="cea40-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cea40-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cea40-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cea40-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="cea40-133">C#</span><span class="sxs-lookup"><span data-stu-id="cea40-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cea40-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cea40-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cea40-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cea40-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cea40-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cea40-136">Response</span></span>

<span data-ttu-id="cea40-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cea40-137">The following is an example of the response.</span></span>
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


