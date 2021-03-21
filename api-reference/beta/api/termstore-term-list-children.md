---
title: Listar filhos
description: Obter os termos da propriedade de navegação para filhos.
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 6bc2ba250498d6d7ac51914e2f0c072a34fc9bfe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955364"
---
# <a name="list-children"></a><span data-ttu-id="912cc-103">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="912cc-103">List children</span></span>
<span data-ttu-id="912cc-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="912cc-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="912cc-105">Obter os filhos de primeiro nível de um [recurso de conjunto] ou [termo] usando a propriedade de navegação filho.</span><span class="sxs-lookup"><span data-stu-id="912cc-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="912cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="912cc-106">Permissions</span></span>
<span data-ttu-id="912cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="912cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="912cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="912cc-109">Permission type</span></span>|<span data-ttu-id="912cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="912cc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="912cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="912cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="912cc-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912cc-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="912cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="912cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="912cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="912cc-114">Not supported.</span></span>    |
|<span data-ttu-id="912cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="912cc-115">Application</span></span> | <span data-ttu-id="912cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="912cc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="912cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="912cc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="912cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="912cc-118">Optional query parameters</span></span>
<span data-ttu-id="912cc-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="912cc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="912cc-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="912cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="912cc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="912cc-121">Request headers</span></span>
|<span data-ttu-id="912cc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="912cc-122">Name</span></span>|<span data-ttu-id="912cc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="912cc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="912cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="912cc-124">Authorization</span></span>|<span data-ttu-id="912cc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="912cc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="912cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="912cc-127">Request body</span></span>
<span data-ttu-id="912cc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="912cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="912cc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="912cc-129">Response</span></span>

<span data-ttu-id="912cc-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="912cc-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="912cc-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="912cc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="912cc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="912cc-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="912cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="912cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term_2"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```
# <a name="c"></a>[<span data-ttu-id="912cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="912cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="912cc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="912cc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="912cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="912cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="912cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="912cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="912cc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="912cc-138">Response</span></span>
<span data-ttu-id="912cc-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="912cc-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.term)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {      
      "id": "81be9856-9856-81be-5698-be815698be81",
      "labels" : [
        {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
        }
      ],
      "lastModifiedDateTime": "2019-06-21T20:01:37Z"
   }  
 ]
}
```

[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get children of a term or termSet in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termchildren",
  "suppressions": []
}
-->


