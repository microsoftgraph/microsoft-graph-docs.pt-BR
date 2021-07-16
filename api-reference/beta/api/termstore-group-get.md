---
title: Obter grupo termStore
description: Leia as propriedades e as relações de um objeto group.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 8f36e8b6b2e03ed9a05294b35736dbbb1b0dd578
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53458963"
---
# <a name="get-termstore-group"></a><span data-ttu-id="8af88-103">Obter grupo termStore</span><span class="sxs-lookup"><span data-stu-id="8af88-103">Get termStore group</span></span>
<span data-ttu-id="8af88-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="8af88-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8af88-105">Leia as propriedades e as relações de um objeto de grupo de armazenamento [de](../resources/termstore-group.md) termos.</span><span class="sxs-lookup"><span data-stu-id="8af88-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8af88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8af88-106">Permissions</span></span>
<span data-ttu-id="8af88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8af88-109">Permission type</span></span>|<span data-ttu-id="8af88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8af88-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8af88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8af88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8af88-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8af88-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="8af88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8af88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8af88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8af88-114">Not supported.</span></span>    |
|<span data-ttu-id="8af88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8af88-115">Application</span></span> | <span data-ttu-id="8af88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8af88-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="8af88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8af88-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{group-id}
GET /sites/{site-id}/termStore/groups/{group-id}
```

## <a name="request-headers"></a><span data-ttu-id="8af88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8af88-118">Request headers</span></span>
|<span data-ttu-id="8af88-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8af88-119">Name</span></span>|<span data-ttu-id="8af88-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af88-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8af88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8af88-121">Authorization</span></span>|<span data-ttu-id="8af88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8af88-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af88-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8af88-124">Request body</span></span>
<span data-ttu-id="8af88-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8af88-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af88-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af88-126">Response</span></span>

<span data-ttu-id="8af88-127">Se tiver êxito, este método retornará um código de `200 OK` resposta e um objeto [microsoft.graph.termStore.group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8af88-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8af88-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8af88-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="8af88-129">Exemplo 1: Obter um grupo termStore</span><span class="sxs-lookup"><span data-stu-id="8af88-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="8af88-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8af88-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8af88-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8af88-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C
```
# <a name="c"></a>[<span data-ttu-id="8af88-132">C#</span><span class="sxs-lookup"><span data-stu-id="8af88-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8af88-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8af88-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8af88-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8af88-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8af88-135">Java</span><span class="sxs-lookup"><span data-stu-id="8af88-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8af88-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af88-136">Response</span></span>

><span data-ttu-id="8af88-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8af88-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="8af88-138">Exemplo 2: Obter um grupo termStore e sua ID de site pai</span><span class="sxs-lookup"><span data-stu-id="8af88-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="8af88-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8af88-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8af88-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8af88-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C?$select=*,parentSiteId
```
# <a name="c"></a>[<span data-ttu-id="8af88-141">C#</span><span class="sxs-lookup"><span data-stu-id="8af88-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8af88-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8af88-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8af88-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8af88-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8af88-144">Java</span><span class="sxs-lookup"><span data-stu-id="8af88-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8af88-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af88-145">Response</span></span>

><span data-ttu-id="8af88-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8af88-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "parentSiteId": "microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f"
}
```

### <a name="example-3-get-a-site-collection-termstore-group"></a><span data-ttu-id="8af88-147">Exemplo 3: Obter um grupo de repositório de termos de conjunto de sites</span><span class="sxs-lookup"><span data-stu-id="8af88-147">Example 3: Get a site collection termStore group</span></span>
#### <a name="request"></a><span data-ttu-id="8af88-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8af88-148">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C
```

#### <a name="response"></a><span data-ttu-id="8af88-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af88-149">Response</span></span>

><span data-ttu-id="8af88-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8af88-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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


