---
title: Obter loja
description: Leia as propriedades e os relacionamentos de um objeto store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fb94dd40644fc1c8ad3f1727fa41b9143f2b1e13
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874414"
---
# <a name="get-store"></a><span data-ttu-id="f6555-103">Obter loja</span><span class="sxs-lookup"><span data-stu-id="f6555-103">Get store</span></span>
<span data-ttu-id="f6555-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="f6555-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6555-105">Leia as propriedades e os relacionamentos de um [objeto store.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="f6555-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6555-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6555-106">Permissions</span></span>
<span data-ttu-id="f6555-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6555-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6555-109">Permission type</span></span>|<span data-ttu-id="f6555-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6555-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6555-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6555-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6555-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6555-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f6555-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6555-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6555-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6555-114">Not supported.</span></span>    |
|<span data-ttu-id="f6555-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6555-115">Application</span></span> | <span data-ttu-id="f6555-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6555-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6555-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6555-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="f6555-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6555-118">Request headers</span></span>
|<span data-ttu-id="f6555-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f6555-119">Name</span></span>|<span data-ttu-id="f6555-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6555-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6555-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6555-121">Authorization</span></span>|<span data-ttu-id="f6555-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6555-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="f6555-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6555-124">Response</span></span>

<span data-ttu-id="f6555-125">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [store](../resources/termstore-store.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6555-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6555-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f6555-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6555-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6555-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6555-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6555-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="f6555-129">C#</span><span class="sxs-lookup"><span data-stu-id="f6555-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6555-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6555-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6555-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6555-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6555-132">Java</span><span class="sxs-lookup"><span data-stu-id="f6555-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f6555-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6555-133">Response</span></span>
<span data-ttu-id="f6555-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f6555-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{  
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag" : "en-US",
  "languageTags" : ["en-US", "de-DE", "fr-FR"]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termStore entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termStore",
  "suppressions": []
}
-->


