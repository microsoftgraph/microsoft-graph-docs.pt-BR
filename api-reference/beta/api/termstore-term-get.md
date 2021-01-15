---
title: Obter termo
description: Leia as propriedades e os relacionamentos de um objeto term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1215ba651f2ff164bdfe414274252be13bf8ff62
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874085"
---
# <a name="get-term"></a><span data-ttu-id="70f58-103">Obter termo</span><span class="sxs-lookup"><span data-stu-id="70f58-103">Get term</span></span>
<span data-ttu-id="70f58-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="70f58-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70f58-105">Leia as propriedades e os relacionamentos de um [objeto term.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="70f58-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70f58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="70f58-106">Permissions</span></span>
<span data-ttu-id="70f58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70f58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70f58-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70f58-109">Permission type</span></span>|<span data-ttu-id="70f58-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70f58-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70f58-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70f58-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70f58-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f58-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="70f58-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70f58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70f58-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70f58-114">Not supported.</span></span>    |
|<span data-ttu-id="70f58-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70f58-115">Application</span></span> | <span data-ttu-id="70f58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70f58-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="70f58-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70f58-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{groupId}/sets/{setId}/terms/{termId}
GET /termStore/sets/{setId}/terms/{termId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70f58-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70f58-118">Optional query parameters</span></span>
<span data-ttu-id="70f58-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70f58-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="70f58-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="70f58-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="70f58-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70f58-121">Request headers</span></span>
|<span data-ttu-id="70f58-122">Nome</span><span class="sxs-lookup"><span data-stu-id="70f58-122">Name</span></span>|<span data-ttu-id="70f58-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="70f58-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70f58-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="70f58-124">Authorization</span></span>|<span data-ttu-id="70f58-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70f58-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70f58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70f58-127">Request body</span></span>
<span data-ttu-id="70f58-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70f58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70f58-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="70f58-129">Response</span></span>

<span data-ttu-id="70f58-130">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70f58-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70f58-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="70f58-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70f58-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70f58-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="70f58-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="70f58-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="70f58-134">C#</span><span class="sxs-lookup"><span data-stu-id="70f58-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70f58-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70f58-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70f58-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70f58-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70f58-137">Java</span><span class="sxs-lookup"><span data-stu-id="70f58-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="70f58-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="70f58-138">Response</span></span>
<span data-ttu-id="70f58-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70f58-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



