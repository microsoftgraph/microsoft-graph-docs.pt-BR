---
title: Obter loja
description: Leia as propriedades e as relações de um objeto store.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 71f23420196bab347cfe74068602b128eada36f4
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456482"
---
# <a name="get-store"></a><span data-ttu-id="37a5b-103">Obter loja</span><span class="sxs-lookup"><span data-stu-id="37a5b-103">Get store</span></span>
<span data-ttu-id="37a5b-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="37a5b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a5b-105">Leia as propriedades e as relações de um [objeto](../resources/termstore-store.md) store.</span><span class="sxs-lookup"><span data-stu-id="37a5b-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37a5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37a5b-106">Permissions</span></span>
<span data-ttu-id="37a5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37a5b-109">Permission type</span></span>|<span data-ttu-id="37a5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37a5b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37a5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37a5b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37a5b-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a5b-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="37a5b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37a5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a5b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a5b-114">Not supported.</span></span>    |
|<span data-ttu-id="37a5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37a5b-115">Application</span></span> | <span data-ttu-id="37a5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a5b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37a5b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37a5b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
GET /sites/{site-id}/termStore
```

## <a name="request-headers"></a><span data-ttu-id="37a5b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37a5b-118">Request headers</span></span>
|<span data-ttu-id="37a5b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37a5b-119">Name</span></span>|<span data-ttu-id="37a5b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a5b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37a5b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37a5b-121">Authorization</span></span>|<span data-ttu-id="37a5b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a5b-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="37a5b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a5b-124">Response</span></span>

<span data-ttu-id="37a5b-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [store](../resources/termstore-store.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37a5b-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37a5b-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37a5b-126">Examples</span></span>

### <a name="example-1-get-a-termstore"></a><span data-ttu-id="37a5b-127">Exemplo 1: Obter um termStore</span><span class="sxs-lookup"><span data-stu-id="37a5b-127">Example 1: Get a termStore</span></span>

#### <a name="request"></a><span data-ttu-id="37a5b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a5b-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="37a5b-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a5b-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="37a5b-130">C#</span><span class="sxs-lookup"><span data-stu-id="37a5b-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a5b-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a5b-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a5b-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a5b-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37a5b-133">Java</span><span class="sxs-lookup"><span data-stu-id="37a5b-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="37a5b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a5b-134">Response</span></span>
><span data-ttu-id="37a5b-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37a5b-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-site-collection-termstore"></a><span data-ttu-id="37a5b-136">Exemplo 2: Obter um conjunto de sites termStore</span><span class="sxs-lookup"><span data-stu-id="37a5b-136">Example 2: Get a site collection termStore</span></span>

#### <a name="request"></a><span data-ttu-id="37a5b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a5b-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore
```

#### <a name="response"></a><span data-ttu-id="37a5b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a5b-138">Response</span></span>
><span data-ttu-id="37a5b-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37a5b-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


