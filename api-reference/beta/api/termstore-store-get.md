---
title: Obter repositório
description: Leia as propriedades e os relacionamentos de um objeto Store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8ed30c99a509f062e7b6f6dc255e1bf08cfbf31b
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565805"
---
# <a name="get-store"></a><span data-ttu-id="91bfa-103">Obter repositório</span><span class="sxs-lookup"><span data-stu-id="91bfa-103">Get store</span></span>
<span data-ttu-id="91bfa-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="91bfa-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91bfa-105">Leia as propriedades e os relacionamentos de um objeto [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="91bfa-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91bfa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="91bfa-106">Permissions</span></span>
<span data-ttu-id="91bfa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91bfa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91bfa-109">Permission type</span></span>|<span data-ttu-id="91bfa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91bfa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91bfa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91bfa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="91bfa-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="91bfa-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="91bfa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91bfa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91bfa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91bfa-114">Not supported.</span></span>    |
|<span data-ttu-id="91bfa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91bfa-115">Application</span></span> | <span data-ttu-id="91bfa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91bfa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91bfa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91bfa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="91bfa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfa-118">Request headers</span></span>
|<span data-ttu-id="91bfa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="91bfa-119">Name</span></span>|<span data-ttu-id="91bfa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bfa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="91bfa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="91bfa-121">Authorization</span></span>|<span data-ttu-id="91bfa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91bfa-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="91bfa-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="91bfa-124">Response</span></span>

<span data-ttu-id="91bfa-125">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Store](../resources/termstore-store.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91bfa-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91bfa-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="91bfa-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91bfa-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfa-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="91bfa-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="91bfa-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="91bfa-129">C#</span><span class="sxs-lookup"><span data-stu-id="91bfa-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91bfa-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91bfa-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91bfa-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91bfa-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="91bfa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="91bfa-132">Response</span></span>
<span data-ttu-id="91bfa-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="91bfa-133">**Note:** The response object shown here might be shortened for readability.</span></span>

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
