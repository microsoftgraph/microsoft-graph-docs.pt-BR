---
title: Excluir siteSource
description: Excluir um objeto siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5948064b4fffa2af858b3e6bfb92eb02f991c784
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445762"
---
# <a name="delete-sitesource"></a><span data-ttu-id="acb0e-103">Excluir siteSource</span><span class="sxs-lookup"><span data-stu-id="acb0e-103">Delete siteSource</span></span>

<span data-ttu-id="acb0e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="acb0e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acb0e-105">Excluir um [objeto siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="acb0e-105">Delete a [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="acb0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="acb0e-106">Permissions</span></span>

<span data-ttu-id="acb0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acb0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acb0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acb0e-109">Permission type</span></span>|<span data-ttu-id="acb0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="acb0e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acb0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acb0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="acb0e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acb0e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="acb0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acb0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acb0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acb0e-114">Not supported.</span></span>|
|<span data-ttu-id="acb0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acb0e-115">Application</span></span>|<span data-ttu-id="acb0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acb0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acb0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acb0e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="acb0e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acb0e-118">Request headers</span></span>

|<span data-ttu-id="acb0e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="acb0e-119">Name</span></span>|<span data-ttu-id="acb0e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb0e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="acb0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="acb0e-121">Authorization</span></span>|<span data-ttu-id="acb0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acb0e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="acb0e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acb0e-124">Request body</span></span>

<span data-ttu-id="acb0e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acb0e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acb0e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="acb0e-126">Response</span></span>

<span data-ttu-id="acb0e-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="acb0e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="acb0e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="acb0e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="acb0e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acb0e-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="acb0e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="acb0e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sitesource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```
# <a name="c"></a>[<span data-ttu-id="acb0e-131">C#</span><span class="sxs-lookup"><span data-stu-id="acb0e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acb0e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acb0e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acb0e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acb0e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acb0e-134">Java</span><span class="sxs-lookup"><span data-stu-id="acb0e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="acb0e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="acb0e-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
