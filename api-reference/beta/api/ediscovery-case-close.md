---
title: 'case: close'
description: Feche um caso de Descoberta e.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 51e9c2164565c46371b7c3ee2d14c30d241354f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773890"
---
# <a name="case-close"></a><span data-ttu-id="23e1f-103">case: close</span><span class="sxs-lookup"><span data-stu-id="23e1f-103">case: close</span></span>

<span data-ttu-id="23e1f-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="23e1f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e1f-105">Feche um caso de Descoberta e.</span><span class="sxs-lookup"><span data-stu-id="23e1f-105">Close an eDiscovery case.</span></span> <span data-ttu-id="23e1f-106">Para obter detalhes, consulte [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span><span class="sxs-lookup"><span data-stu-id="23e1f-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="23e1f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="23e1f-107">Permissions</span></span>

<span data-ttu-id="23e1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23e1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23e1f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23e1f-110">Permission type</span></span>|<span data-ttu-id="23e1f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23e1f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23e1f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23e1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23e1f-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e1f-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="23e1f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23e1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23e1f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23e1f-115">Not supported.</span></span>|
|<span data-ttu-id="23e1f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23e1f-116">Application</span></span>|<span data-ttu-id="23e1f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23e1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e1f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23e1f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{CaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="23e1f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23e1f-119">Request headers</span></span>

|<span data-ttu-id="23e1f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="23e1f-120">Name</span></span>|<span data-ttu-id="23e1f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23e1f-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23e1f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23e1f-122">Authorization</span></span>|<span data-ttu-id="23e1f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23e1f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23e1f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23e1f-125">Request body</span></span>

<span data-ttu-id="23e1f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23e1f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23e1f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="23e1f-127">Response</span></span>

<span data-ttu-id="23e1f-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23e1f-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="23e1f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23e1f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23e1f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23e1f-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="23e1f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="23e1f-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```

# <a name="c"></a>[<span data-ttu-id="23e1f-132">C#</span><span class="sxs-lookup"><span data-stu-id="23e1f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/case-close-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-close-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23e1f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23e1f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/case-close-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-close-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23e1f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23e1f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/case-close-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-close-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23e1f-135">Java</span><span class="sxs-lookup"><span data-stu-id="23e1f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/case-close-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-close-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="23e1f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="23e1f-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
