---
title: Obter grupo
description: Leia as propriedades e as relações de um objeto group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2c95937181d90a2f1b8759464b7ef8506397c4a1
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507155"
---
# <a name="get-group"></a><span data-ttu-id="cbc39-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="cbc39-103">Get group</span></span>
<span data-ttu-id="cbc39-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="cbc39-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbc39-105">Leia as propriedades e as relações de um objeto de grupo de armazenamento [de](../resources/termstore-group.md) termos.</span><span class="sxs-lookup"><span data-stu-id="cbc39-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbc39-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cbc39-106">Permissions</span></span>
<span data-ttu-id="cbc39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc39-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbc39-109">Permission type</span></span>|<span data-ttu-id="cbc39-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbc39-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbc39-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbc39-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cbc39-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbc39-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="cbc39-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbc39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbc39-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc39-114">Not supported.</span></span>    |
|<span data-ttu-id="cbc39-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbc39-115">Application</span></span> | <span data-ttu-id="cbc39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc39-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="cbc39-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc39-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="cbc39-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc39-118">Request headers</span></span>
|<span data-ttu-id="cbc39-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cbc39-119">Name</span></span>|<span data-ttu-id="cbc39-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbc39-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cbc39-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbc39-121">Authorization</span></span>|<span data-ttu-id="cbc39-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbc39-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbc39-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc39-124">Request body</span></span>
<span data-ttu-id="cbc39-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbc39-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbc39-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc39-126">Response</span></span>

<span data-ttu-id="cbc39-127">Se tiver êxito, este método retornará um código de `200 OK` resposta e um objeto [microsoft.graph.termStore.group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbc39-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cbc39-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cbc39-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="cbc39-129">Exemplo 1: Obter um grupo termStore</span><span class="sxs-lookup"><span data-stu-id="cbc39-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="cbc39-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc39-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cbc39-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc39-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="cbc39-132">C#</span><span class="sxs-lookup"><span data-stu-id="cbc39-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbc39-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbc39-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbc39-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbc39-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cbc39-135">Java</span><span class="sxs-lookup"><span data-stu-id="cbc39-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cbc39-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc39-136">Response</span></span>

<span data-ttu-id="cbc39-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cbc39-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup"  
}
```
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="cbc39-138">Exemplo 2: Obter um grupo termStore e sua ID de site pai</span><span class="sxs-lookup"><span data-stu-id="cbc39-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="cbc39-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc39-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cbc39-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc39-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}?$select=*,parentSiteId
```
# <a name="c"></a>[<span data-ttu-id="cbc39-141">C#</span><span class="sxs-lookup"><span data-stu-id="cbc39-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbc39-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbc39-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbc39-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbc39-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cbc39-144">Java</span><span class="sxs-lookup"><span data-stu-id="cbc39-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cbc39-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc39-145">Response</span></span>

<span data-ttu-id="cbc39-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cbc39-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup",
  "parentSiteId": "microsoft.sharepoint.com,05259ba9-25a8-4c93-a9a9-f995ef1fc51f,a785ad58-1d57-4f8a-aa71-77170459bd0d"
}
```

[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termGroup",
  "suppressions": [
  ]
}
-->


