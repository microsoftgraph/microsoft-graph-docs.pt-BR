---
title: Excluir marca
description: Exclua um objeto tag.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8c21df5939cde9b707dd913dbfa383ba1e950d53
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776456"
---
# <a name="delete-tag"></a><span data-ttu-id="c2608-103">Excluir marca</span><span class="sxs-lookup"><span data-stu-id="c2608-103">Delete tag</span></span>

<span data-ttu-id="c2608-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c2608-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2608-105">Exclua [um objeto tag.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="c2608-105">Delete a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2608-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2608-106">Permissions</span></span>

<span data-ttu-id="c2608-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2608-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2608-109">Permission type</span></span>|<span data-ttu-id="c2608-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2608-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2608-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2608-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2608-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2608-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c2608-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2608-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2608-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2608-114">Not supported.</span></span>|
|<span data-ttu-id="c2608-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2608-115">Application</span></span>|<span data-ttu-id="c2608-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2608-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2608-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2608-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/tags/{tagId}?forcedelete=true
```

## <a name="query-parameters"></a><span data-ttu-id="c2608-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="c2608-118">Query parameters</span></span>

<span data-ttu-id="c2608-119">Na URL de solicitação, forneça o seguinte parâmetro de consulta necessário.</span><span class="sxs-lookup"><span data-stu-id="c2608-119">In the request URL, provide the following required query parameter.</span></span>

| <span data-ttu-id="c2608-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c2608-120">Parameter</span></span>     | <span data-ttu-id="c2608-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2608-121">Type</span></span>    | <span data-ttu-id="c2608-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2608-122">Description</span></span>                                                                              |
|:--------------|:--------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="c2608-123">forcedelete</span><span class="sxs-lookup"><span data-stu-id="c2608-123">forcedelete</span></span>   | <span data-ttu-id="c2608-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="c2608-124">Boolean</span></span> | <span data-ttu-id="c2608-125">Se definido como true, a marca e os filhos serão excluídos, se false, e a marca tiver filhos, a exclusão falhará.</span><span class="sxs-lookup"><span data-stu-id="c2608-125">If set to true, the tag and children will be deleted, if false, and the tag has children, the delete will fail.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c2608-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2608-126">Request headers</span></span>

|<span data-ttu-id="c2608-127">Nome</span><span class="sxs-lookup"><span data-stu-id="c2608-127">Name</span></span>|<span data-ttu-id="c2608-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2608-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c2608-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2608-129">Authorization</span></span>|<span data-ttu-id="c2608-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2608-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2608-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2608-132">Request body</span></span>

<span data-ttu-id="c2608-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2608-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2608-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2608-134">Response</span></span>

<span data-ttu-id="c2608-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2608-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c2608-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c2608-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2608-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2608-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2608-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2608-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tag"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true
```
# <a name="c"></a>[<span data-ttu-id="c2608-139">C#</span><span class="sxs-lookup"><span data-stu-id="c2608-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2608-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2608-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2608-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2608-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2608-142">Java</span><span class="sxs-lookup"><span data-stu-id="c2608-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2608-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2608-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
