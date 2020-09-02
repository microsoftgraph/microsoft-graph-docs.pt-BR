---
title: Obter termo
description: Leia as propriedades e os relacionamentos de um objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5d154606c4f3581f0c5136ebd04d863185cf1721
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330159"
---
# <a name="get-term"></a><span data-ttu-id="65ebf-103">Obter termo</span><span class="sxs-lookup"><span data-stu-id="65ebf-103">Get term</span></span>
<span data-ttu-id="65ebf-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="65ebf-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65ebf-105">Leia as propriedades e os relacionamentos de um objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="65ebf-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65ebf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65ebf-106">Permissions</span></span>
<span data-ttu-id="65ebf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ebf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65ebf-109">Permission type</span></span>|<span data-ttu-id="65ebf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65ebf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65ebf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65ebf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="65ebf-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="65ebf-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="65ebf-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65ebf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65ebf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65ebf-114">Not supported.</span></span>    |
|<span data-ttu-id="65ebf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65ebf-115">Application</span></span> | <span data-ttu-id="65ebf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65ebf-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="65ebf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65ebf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{groupId}/sets/{setId}/terms/{termId}
GET /termStore/sets/{setId}/terms/{termId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65ebf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65ebf-118">Optional query parameters</span></span>
<span data-ttu-id="65ebf-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65ebf-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="65ebf-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="65ebf-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="65ebf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65ebf-121">Request headers</span></span>
|<span data-ttu-id="65ebf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="65ebf-122">Name</span></span>|<span data-ttu-id="65ebf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="65ebf-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65ebf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="65ebf-124">Authorization</span></span>|<span data-ttu-id="65ebf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65ebf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65ebf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65ebf-127">Request body</span></span>
<span data-ttu-id="65ebf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65ebf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65ebf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ebf-129">Response</span></span>

<span data-ttu-id="65ebf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65ebf-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65ebf-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="65ebf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65ebf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65ebf-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65ebf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="65ebf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="65ebf-134">C#</span><span class="sxs-lookup"><span data-stu-id="65ebf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65ebf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65ebf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65ebf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65ebf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="65ebf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ebf-137">Response</span></span>
<span data-ttu-id="65ebf-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65ebf-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

