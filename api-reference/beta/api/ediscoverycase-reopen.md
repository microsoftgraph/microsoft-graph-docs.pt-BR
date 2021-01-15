---
title: 'ediscoveryCase: reopen'
description: Reabra um caso de Descoberta e Que foi fechado.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f8eb4265fb87668023038ddaa50967cad22c2a91
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872293"
---
# <a name="ediscoverycase-reopen"></a><span data-ttu-id="f8487-103">ediscoveryCase: reopen</span><span class="sxs-lookup"><span data-stu-id="f8487-103">ediscoveryCase: reopen</span></span>

<span data-ttu-id="f8487-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8487-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8487-105">Reabra um caso de Descoberta e Que foi fechado.</span><span class="sxs-lookup"><span data-stu-id="f8487-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="f8487-106">Para obter detalhes, consulte [Reabrir um caso fechado.](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case)</span><span class="sxs-lookup"><span data-stu-id="f8487-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8487-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8487-107">Permissions</span></span>
<span data-ttu-id="f8487-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8487-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8487-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8487-110">Permission type</span></span>|<span data-ttu-id="f8487-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8487-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8487-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8487-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8487-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="f8487-113">User.Read</span></span>|
|<span data-ttu-id="f8487-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8487-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8487-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8487-115">Not supported.</span></span>|
|<span data-ttu-id="f8487-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8487-116">Application</span></span>|<span data-ttu-id="f8487-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8487-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8487-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8487-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="f8487-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8487-119">Request headers</span></span>

|<span data-ttu-id="f8487-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f8487-120">Name</span></span>|<span data-ttu-id="f8487-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8487-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8487-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8487-122">Authorization</span></span>|<span data-ttu-id="f8487-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8487-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8487-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8487-125">Request body</span></span>

<span data-ttu-id="f8487-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8487-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8487-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8487-127">Response</span></span>

<span data-ttu-id="f8487-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8487-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f8487-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8487-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8487-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8487-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f8487-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8487-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycase_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="f8487-132">C#</span><span class="sxs-lookup"><span data-stu-id="f8487-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8487-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8487-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8487-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8487-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8487-135">Java</span><span class="sxs-lookup"><span data-stu-id="f8487-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8487-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8487-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
