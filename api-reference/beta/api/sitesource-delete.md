---
title: Excluir site local
description: Excluir um objeto de site.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c4732e101fe86fdd9cafbad658bf1e3211283514
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659560"
---
# <a name="delete-sitesource"></a><span data-ttu-id="42505-103">Excluir site local</span><span class="sxs-lookup"><span data-stu-id="42505-103">Delete siteSource</span></span>

<span data-ttu-id="42505-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42505-105">Excluir um objeto de [site](../resources/sitesource.md) .</span><span class="sxs-lookup"><span data-stu-id="42505-105">Delete a [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42505-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42505-106">Permissions</span></span>

<span data-ttu-id="42505-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42505-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42505-109">Permission type</span></span>|<span data-ttu-id="42505-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42505-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42505-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42505-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42505-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="42505-112">User.Read</span></span>|
|<span data-ttu-id="42505-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42505-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42505-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42505-114">Not supported.</span></span>|
|<span data-ttu-id="42505-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42505-115">Application</span></span>|<span data-ttu-id="42505-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42505-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42505-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42505-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="42505-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42505-118">Request headers</span></span>

|<span data-ttu-id="42505-119">Nome</span><span class="sxs-lookup"><span data-stu-id="42505-119">Name</span></span>|<span data-ttu-id="42505-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42505-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="42505-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42505-121">Authorization</span></span>|<span data-ttu-id="42505-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42505-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42505-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42505-124">Request body</span></span>

<span data-ttu-id="42505-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42505-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42505-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="42505-126">Response</span></span>

<span data-ttu-id="42505-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42505-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="42505-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42505-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42505-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42505-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="42505-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="42505-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sitesource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```
# <a name="c"></a>[<span data-ttu-id="42505-131">C#</span><span class="sxs-lookup"><span data-stu-id="42505-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42505-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42505-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42505-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42505-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42505-134">Java</span><span class="sxs-lookup"><span data-stu-id="42505-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42505-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="42505-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
