---
title: Obter grupo
description: Leia as propriedades e as relações de um objeto group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e13a7d3f79da8227e0599d30182ea30e6799ed96
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961326"
---
# <a name="get-group"></a><span data-ttu-id="31026-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="31026-103">Get group</span></span>
<span data-ttu-id="31026-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="31026-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31026-105">Leia as propriedades e as relações de um [objeto group.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="31026-105">Read the properties and relationships of a [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31026-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31026-106">Permissions</span></span>
<span data-ttu-id="31026-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31026-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31026-109">Permission type</span></span>|<span data-ttu-id="31026-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31026-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31026-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31026-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31026-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31026-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="31026-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31026-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31026-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31026-114">Not supported.</span></span>    |
|<span data-ttu-id="31026-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31026-115">Application</span></span> | <span data-ttu-id="31026-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31026-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="31026-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31026-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="31026-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31026-118">Request headers</span></span>
|<span data-ttu-id="31026-119">Nome</span><span class="sxs-lookup"><span data-stu-id="31026-119">Name</span></span>|<span data-ttu-id="31026-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="31026-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31026-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="31026-121">Authorization</span></span>|<span data-ttu-id="31026-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31026-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31026-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31026-124">Request body</span></span>
<span data-ttu-id="31026-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31026-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31026-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="31026-126">Response</span></span>

<span data-ttu-id="31026-127">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31026-127">If successful, this method returns a `200 OK` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31026-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31026-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31026-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31026-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="31026-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="31026-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="31026-131">C#</span><span class="sxs-lookup"><span data-stu-id="31026-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31026-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31026-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31026-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31026-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31026-134">Java</span><span class="sxs-lookup"><span data-stu-id="31026-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="31026-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="31026-135">Response</span></span>

<span data-ttu-id="31026-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31026-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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


