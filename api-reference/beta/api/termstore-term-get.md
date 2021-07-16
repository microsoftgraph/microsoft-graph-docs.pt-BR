---
title: Obter termo
description: Leia as propriedades e as relações de um objeto term.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: b26b1bc5da13bd8edabe3f381f950c47894800d2
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456475"
---
# <a name="get-term"></a><span data-ttu-id="a4c63-103">Obter termo</span><span class="sxs-lookup"><span data-stu-id="a4c63-103">Get term</span></span>
<span data-ttu-id="a4c63-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="a4c63-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4c63-105">Leia as propriedades e as relações de um [objeto term.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="a4c63-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4c63-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4c63-106">Permissions</span></span>
<span data-ttu-id="a4c63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4c63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4c63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4c63-109">Permission type</span></span>|<span data-ttu-id="a4c63-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4c63-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4c63-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4c63-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4c63-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4c63-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="a4c63-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4c63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4c63-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c63-114">Not supported.</span></span>    |
|<span data-ttu-id="a4c63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4c63-115">Application</span></span> | <span data-ttu-id="a4c63-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c63-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a4c63-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c63-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{group-id}/sets/{set-id}/terms/{term-id}
GET /termStore/sets/{set-id}/terms/{term-id}
GET /sites/{site-id}/termStore/groups/{group-id}/sets/{set-id}/terms/{term-id}
GET /sites/{site-id}/termStore/sets/{set-id}/terms/{term-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4c63-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4c63-118">Optional query parameters</span></span>
<span data-ttu-id="a4c63-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c63-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a4c63-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a4c63-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4c63-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c63-121">Request headers</span></span>
|<span data-ttu-id="a4c63-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a4c63-122">Name</span></span>|<span data-ttu-id="a4c63-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4c63-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4c63-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4c63-124">Authorization</span></span>|<span data-ttu-id="a4c63-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4c63-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4c63-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c63-127">Request body</span></span>
<span data-ttu-id="a4c63-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4c63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4c63-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c63-129">Response</span></span>

<span data-ttu-id="a4c63-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c63-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4c63-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4c63-131">Examples</span></span>

### <a name="example-1-get-a-termstore-term"></a><span data-ttu-id="a4c63-132">Exemplo 1: Obter um termo termStore</span><span class="sxs-lookup"><span data-stu-id="a4c63-132">Example 1: Get a termStore term</span></span>

#### <a name="request"></a><span data-ttu-id="a4c63-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c63-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4c63-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c63-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81
```
# <a name="c"></a>[<span data-ttu-id="a4c63-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4c63-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4c63-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4c63-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4c63-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4c63-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4c63-138">Java</span><span class="sxs-lookup"><span data-stu-id="a4c63-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a4c63-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c63-139">Response</span></span>
><span data-ttu-id="a4c63-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4c63-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "labels" : [
    {
        "name" : "Copy of myTerm",
        "languageTag" : "en-US",
        "isDefault" : true
    }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```
### <a name="example-2--get-a-site-collection-termstore-term"></a><span data-ttu-id="a4c63-141">Exemplo 2: Obter um termo de repositório de conjunto de sites</span><span class="sxs-lookup"><span data-stu-id="a4c63-141">Example 2 : Get a site collection termStore term</span></span>

#### <a name="request"></a><span data-ttu-id="a4c63-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c63-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81
```

#### <a name="response"></a><span data-ttu-id="a4c63-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c63-143">Response</span></span>
><span data-ttu-id="a4c63-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4c63-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "labels" : [
    {
        "name" : "Copy of myTerm",
        "languageTag" : "en-US",
        "isDefault" : true
    }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get term",
  "suppressions": [
  ]
}
-->



