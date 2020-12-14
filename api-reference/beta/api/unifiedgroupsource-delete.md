---
title: Excluir unifiedGroupSource
description: Excluir um objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 09afb8ed8e91787df7647fb366de55f96a481a83
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657141"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="5b5f1-103">Excluir unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5b5f1-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="5b5f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b5f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b5f1-105">Excluir um objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="5b5f1-105">Delete a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b5f1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b5f1-106">Permissions</span></span>

<span data-ttu-id="5b5f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b5f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b5f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b5f1-109">Permission type</span></span>|<span data-ttu-id="5b5f1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b5f1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b5f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b5f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b5f1-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="5b5f1-112">User.Read</span></span>|
|<span data-ttu-id="5b5f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b5f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b5f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b5f1-114">Not supported.</span></span>|
|<span data-ttu-id="5b5f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b5f1-115">Application</span></span>|<span data-ttu-id="5b5f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b5f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b5f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b5f1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="5b5f1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b5f1-118">Request headers</span></span>

|<span data-ttu-id="5b5f1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5b5f1-119">Name</span></span>|<span data-ttu-id="5b5f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b5f1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b5f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b5f1-121">Authorization</span></span>|<span data-ttu-id="5b5f1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b5f1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b5f1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b5f1-124">Request body</span></span>

<span data-ttu-id="5b5f1-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b5f1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b5f1-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b5f1-126">Response</span></span>

<span data-ttu-id="5b5f1-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b5f1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5b5f1-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b5f1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b5f1-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b5f1-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5b5f1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b5f1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```
# <a name="c"></a>[<span data-ttu-id="5b5f1-131">C#</span><span class="sxs-lookup"><span data-stu-id="5b5f1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b5f1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b5f1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b5f1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b5f1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b5f1-134">Java</span><span class="sxs-lookup"><span data-stu-id="5b5f1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b5f1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b5f1-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
