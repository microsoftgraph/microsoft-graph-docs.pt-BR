---
title: Obter grupo
description: Leia as propriedades e as relações de um objeto group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 86a96855c330e581e98da902b5e38f16cc857ec9
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473294"
---
# <a name="get-group"></a><span data-ttu-id="cdc49-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="cdc49-103">Get group</span></span>
<span data-ttu-id="cdc49-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="cdc49-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc49-105">Leia as propriedades e as relações de um objeto de grupo de armazenamento [de](../resources/termstore-group.md) termos.</span><span class="sxs-lookup"><span data-stu-id="cdc49-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc49-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdc49-106">Permissions</span></span>
<span data-ttu-id="cdc49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc49-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdc49-109">Permission type</span></span>|<span data-ttu-id="cdc49-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdc49-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc49-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdc49-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdc49-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc49-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="cdc49-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdc49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdc49-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc49-114">Not supported.</span></span>    |
|<span data-ttu-id="cdc49-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdc49-115">Application</span></span> | <span data-ttu-id="cdc49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc49-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="cdc49-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc49-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="cdc49-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc49-118">Request headers</span></span>
|<span data-ttu-id="cdc49-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cdc49-119">Name</span></span>|<span data-ttu-id="cdc49-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc49-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cdc49-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdc49-121">Authorization</span></span>|<span data-ttu-id="cdc49-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdc49-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc49-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc49-124">Request body</span></span>
<span data-ttu-id="cdc49-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdc49-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc49-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc49-126">Response</span></span>

<span data-ttu-id="cdc49-127">Se tiver êxito, este método retornará um código de `200 OK` resposta e um objeto [microsoft.graph.termStore.group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc49-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdc49-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cdc49-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="cdc49-129">Exemplo 1: Obter um grupo termStore</span><span class="sxs-lookup"><span data-stu-id="cdc49-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="cdc49-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc49-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cdc49-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc49-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="cdc49-132">C#</span><span class="sxs-lookup"><span data-stu-id="cdc49-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc49-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc49-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc49-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc49-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc49-135">Java</span><span class="sxs-lookup"><span data-stu-id="cdc49-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cdc49-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc49-136">Response</span></span>

<span data-ttu-id="cdc49-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cdc49-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="cdc49-138">Exemplo 2: Obter um grupo termStore e sua ID de site pai</span><span class="sxs-lookup"><span data-stu-id="cdc49-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="cdc49-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc49-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}?$select=*,parentSiteId
```

#### <a name="response"></a><span data-ttu-id="cdc49-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc49-140">Response</span></span>

<span data-ttu-id="cdc49-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cdc49-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


