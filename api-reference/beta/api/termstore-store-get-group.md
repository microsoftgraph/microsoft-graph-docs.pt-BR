---
title: Obter grupo
description: Leia as propriedades e os relacionamentos de um objeto de grupo.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 71109297be1cbceb41fb83733993505e7a9ea53d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058617"
---
# <a name="get-group"></a><span data-ttu-id="6276f-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="6276f-103">Get group</span></span>
<span data-ttu-id="6276f-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="6276f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6276f-105">Leia as propriedades e os relacionamentos de um objeto de [grupo](../resources/termstore-group.md) .</span><span class="sxs-lookup"><span data-stu-id="6276f-105">Read the properties and relationships of a [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6276f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6276f-106">Permissions</span></span>
<span data-ttu-id="6276f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6276f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6276f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6276f-109">Permission type</span></span>|<span data-ttu-id="6276f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6276f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6276f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6276f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6276f-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6276f-112">TermStore.Read.All,TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="6276f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6276f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6276f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6276f-114">Not supported.</span></span>    |
|<span data-ttu-id="6276f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6276f-115">Application</span></span> | <span data-ttu-id="6276f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6276f-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="6276f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6276f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="6276f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6276f-118">Request headers</span></span>
|<span data-ttu-id="6276f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6276f-119">Name</span></span>|<span data-ttu-id="6276f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6276f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6276f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6276f-121">Authorization</span></span>|<span data-ttu-id="6276f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6276f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6276f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6276f-124">Request body</span></span>
<span data-ttu-id="6276f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6276f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6276f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6276f-126">Response</span></span>

<span data-ttu-id="6276f-127">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6276f-127">If successful, this method returns a `200 OK` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6276f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6276f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6276f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6276f-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6276f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6276f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="6276f-131">C#</span><span class="sxs-lookup"><span data-stu-id="6276f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6276f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6276f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6276f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6276f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6276f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6276f-134">Response</span></span>

<span data-ttu-id="6276f-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6276f-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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


