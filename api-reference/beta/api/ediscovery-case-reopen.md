---
title: 'case: reabrir'
description: Reabra um caso de Descoberta e Que foi fechado.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5eaa03b81502273e6aae914fa699311457df9cd9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445821"
---
# <a name="case-reopen"></a><span data-ttu-id="f5209-103">case: reabrir</span><span class="sxs-lookup"><span data-stu-id="f5209-103">case: reopen</span></span>

<span data-ttu-id="f5209-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f5209-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5209-105">Reabra um caso de Descoberta e Que foi fechado.</span><span class="sxs-lookup"><span data-stu-id="f5209-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="f5209-106">Para obter detalhes, consulte [Reabrar um caso fechado](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span><span class="sxs-lookup"><span data-stu-id="f5209-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5209-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5209-107">Permissions</span></span>

<span data-ttu-id="f5209-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5209-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5209-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5209-110">Permission type</span></span>|<span data-ttu-id="f5209-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5209-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5209-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5209-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5209-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5209-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f5209-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5209-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5209-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5209-115">Not supported.</span></span>|
|<span data-ttu-id="f5209-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5209-116">Application</span></span>|<span data-ttu-id="f5209-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5209-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5209-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5209-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="f5209-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5209-119">Request headers</span></span>

|<span data-ttu-id="f5209-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f5209-120">Name</span></span>|<span data-ttu-id="f5209-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5209-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5209-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5209-122">Authorization</span></span>|<span data-ttu-id="f5209-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5209-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5209-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5209-125">Request body</span></span>

<span data-ttu-id="f5209-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5209-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5209-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5209-127">Response</span></span>

<span data-ttu-id="f5209-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5209-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f5209-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5209-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5209-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5209-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f5209-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5209-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="f5209-132">C#</span><span class="sxs-lookup"><span data-stu-id="f5209-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5209-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5209-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5209-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5209-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5209-135">Java</span><span class="sxs-lookup"><span data-stu-id="f5209-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f5209-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5209-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
