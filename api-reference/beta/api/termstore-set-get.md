---
title: Obter conjunto
description: Leia as propriedades e as relações de um objeto set.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 995ed341a5b92e11f6ecfa7cac8405ec7dc2a2af
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456461"
---
# <a name="get-set"></a><span data-ttu-id="46a17-103">Obter conjunto</span><span class="sxs-lookup"><span data-stu-id="46a17-103">Get set</span></span>
<span data-ttu-id="46a17-104">Namespace: microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="46a17-104">Namespace: microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="46a17-105">Leia as propriedades e as relações de um [objeto set.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="46a17-105">Read the properties and relationships of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46a17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46a17-106">Permissions</span></span>
<span data-ttu-id="46a17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46a17-109">Permission type</span></span>|<span data-ttu-id="46a17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46a17-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46a17-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46a17-111">Delegated (work or school account)</span></span> |<span data-ttu-id="46a17-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a17-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="46a17-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46a17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a17-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46a17-114">Not supported.</span></span>    |
|<span data-ttu-id="46a17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46a17-115">Application</span></span> | <span data-ttu-id="46a17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46a17-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="46a17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46a17-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/sets/{set-id}
GET /sites/{site-id}/termStore/sets/{set-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46a17-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46a17-118">Optional query parameters</span></span>
<span data-ttu-id="46a17-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46a17-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="46a17-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="46a17-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46a17-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46a17-121">Request headers</span></span>
|<span data-ttu-id="46a17-122">Nome</span><span class="sxs-lookup"><span data-stu-id="46a17-122">Name</span></span>|<span data-ttu-id="46a17-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="46a17-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46a17-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="46a17-124">Authorization</span></span>|<span data-ttu-id="46a17-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46a17-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a17-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46a17-127">Request body</span></span>
<span data-ttu-id="46a17-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46a17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a17-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a17-129">Response</span></span>

<span data-ttu-id="46a17-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [set](../resources/termstore-set.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46a17-130">If successful, this method returns a `200 OK` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46a17-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46a17-131">Examples</span></span>

### <a name="example-1-get-a-termstore-set"></a><span data-ttu-id="46a17-132">Exemplo 1: Obter um conjunto termStore</span><span class="sxs-lookup"><span data-stu-id="46a17-132">Example 1: Get a termStore set</span></span>

#### <a name="request"></a><span data-ttu-id="46a17-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46a17-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_set_2"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f
```
# <a name="c"></a>[<span data-ttu-id="46a17-134">C#</span><span class="sxs-lookup"><span data-stu-id="46a17-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46a17-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46a17-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46a17-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46a17-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46a17-137">Java</span><span class="sxs-lookup"><span data-stu-id="46a17-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-set-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="46a17-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a17-138">Response</span></span>
><span data-ttu-id="46a17-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46a17-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

### <a name="example-2-get-a-site-collection-termstore-set"></a><span data-ttu-id="46a17-140">Exemplo 2: Obter um conjunto de sites termoStore Set</span><span class="sxs-lookup"><span data-stu-id="46a17-140">Example 2: Get a site collection termStore Set</span></span>

#### <a name="request"></a><span data-ttu-id="46a17-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46a17-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_siteCollection_termStore_set"
}-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f
```

#### <a name="response"></a><span data-ttu-id="46a17-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a17-142">Response</span></span>
><span data-ttu-id="46a17-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46a17-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termSet",
  "suppressions": [
  ]
}
-->


