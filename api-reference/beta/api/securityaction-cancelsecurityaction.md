---
title: 'securityAction: cancelSecurityAction'
description: Cancele uma operação de segurança.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 41cec1694baa05b67791a000215f44c6cfd8c859
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787230"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="4bd63-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="4bd63-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="4bd63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bd63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bd63-105">Cancele uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="4bd63-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bd63-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4bd63-106">Permissions</span></span>

<span data-ttu-id="4bd63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bd63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bd63-109">Permission type</span></span>                        | <span data-ttu-id="4bd63-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bd63-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4bd63-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bd63-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bd63-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bd63-112">Not supported.</span></span> |
| <span data-ttu-id="4bd63-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bd63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd63-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bd63-114">Not supported.</span></span> |
| <span data-ttu-id="4bd63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bd63-115">Application</span></span>                            | <span data-ttu-id="4bd63-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bd63-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bd63-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd63-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="4bd63-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd63-118">Request headers</span></span>

| <span data-ttu-id="4bd63-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4bd63-119">Name</span></span>          | <span data-ttu-id="4bd63-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bd63-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4bd63-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd63-121">Authorization</span></span> | <span data-ttu-id="4bd63-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4bd63-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bd63-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd63-123">Request body</span></span>

<span data-ttu-id="4bd63-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bd63-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bd63-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bd63-125">Response</span></span>

<span data-ttu-id="4bd63-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bd63-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bd63-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4bd63-128">Examples</span></span>

<span data-ttu-id="4bd63-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4bd63-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4bd63-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd63-130">Request</span></span>

<span data-ttu-id="4bd63-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bd63-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bd63-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd63-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="4bd63-133">C#</span><span class="sxs-lookup"><span data-stu-id="4bd63-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bd63-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bd63-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bd63-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bd63-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4bd63-136">Java</span><span class="sxs-lookup"><span data-stu-id="4bd63-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4bd63-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bd63-137">Response</span></span>

<span data-ttu-id="4bd63-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bd63-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


