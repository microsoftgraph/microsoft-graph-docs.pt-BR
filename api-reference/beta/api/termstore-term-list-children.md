---
title: Listar filhos
description: Obtenha os termos da propriedade de navegação Children.
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: f285feacf48be3ae9cc5e6a987e578aab7978e15
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972253"
---
# <a name="list-children"></a><span data-ttu-id="015ff-103">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="015ff-103">List children</span></span>
<span data-ttu-id="015ff-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="015ff-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="015ff-105">Obter o primeiro nível filho de um recurso [set] ou [Term] usando a propriedade de navegação Children.</span><span class="sxs-lookup"><span data-stu-id="015ff-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="015ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="015ff-106">Permissions</span></span>
<span data-ttu-id="015ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="015ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="015ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="015ff-109">Permission type</span></span>|<span data-ttu-id="015ff-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="015ff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="015ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="015ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="015ff-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="015ff-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="015ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="015ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="015ff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="015ff-114">Not supported.</span></span>    |
|<span data-ttu-id="015ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="015ff-115">Application</span></span> | <span data-ttu-id="015ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="015ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="015ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="015ff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="015ff-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="015ff-118">Optional query parameters</span></span>
<span data-ttu-id="015ff-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="015ff-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="015ff-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="015ff-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="015ff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="015ff-121">Request headers</span></span>
|<span data-ttu-id="015ff-122">Nome</span><span class="sxs-lookup"><span data-stu-id="015ff-122">Name</span></span>|<span data-ttu-id="015ff-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="015ff-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="015ff-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="015ff-124">Authorization</span></span>|<span data-ttu-id="015ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="015ff-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="015ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="015ff-127">Request body</span></span>
<span data-ttu-id="015ff-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="015ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="015ff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="015ff-129">Response</span></span>

<span data-ttu-id="015ff-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="015ff-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="015ff-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="015ff-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="015ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="015ff-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="015ff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="015ff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```
# <a name="c"></a>[<span data-ttu-id="015ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="015ff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="015ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="015ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="015ff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="015ff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="015ff-137">Java</span><span class="sxs-lookup"><span data-stu-id="015ff-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="015ff-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="015ff-138">Response</span></span>
<span data-ttu-id="015ff-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="015ff-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

[terminal]: ../resources/termstore-term.md
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


