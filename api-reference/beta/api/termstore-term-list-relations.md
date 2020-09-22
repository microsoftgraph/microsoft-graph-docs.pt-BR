---
title: Listar relações
description: Obtenha as relações da propriedade de navegação Relations.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ba593b7d5be184d5a53c0dd2af98dc655a3712bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042853"
---
# <a name="list-relations"></a><span data-ttu-id="0613d-103">Listar relações</span><span class="sxs-lookup"><span data-stu-id="0613d-103">List relations</span></span>
<span data-ttu-id="0613d-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="0613d-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0613d-105">Obtenha a relação diferente de um [termo] ou [conjunto] na propriedade de navegação de relações.</span><span class="sxs-lookup"><span data-stu-id="0613d-105">Get the different relation of a [term] or [set] from the relations navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0613d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0613d-106">Permissions</span></span>
<span data-ttu-id="0613d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0613d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0613d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0613d-109">Permission type</span></span>|<span data-ttu-id="0613d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0613d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0613d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0613d-111">Delegated (work or school account)</span></span> |<span data-ttu-id="0613d-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0613d-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="0613d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0613d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0613d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0613d-114">Not supported.</span></span>    |
|<span data-ttu-id="0613d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0613d-115">Application</span></span> | <span data-ttu-id="0613d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0613d-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="0613d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0613d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/relations
GET /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0613d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0613d-118">Optional query parameters</span></span>
<span data-ttu-id="0613d-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0613d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0613d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0613d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0613d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0613d-121">Request headers</span></span>
|<span data-ttu-id="0613d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0613d-122">Name</span></span>|<span data-ttu-id="0613d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0613d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0613d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0613d-124">Authorization</span></span>|<span data-ttu-id="0613d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0613d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0613d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0613d-127">Request body</span></span>
<span data-ttu-id="0613d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0613d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0613d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0613d-129">Response</span></span>

<span data-ttu-id="0613d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [relation](../resources/termstore-relation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0613d-130">If successful, this method returns a `200 OK` response code and a collection of [relation](../resources/termstore-relation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0613d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0613d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0613d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0613d-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0613d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0613d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relation"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/relations
```
# <a name="c"></a>[<span data-ttu-id="0613d-134">C#</span><span class="sxs-lookup"><span data-stu-id="0613d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0613d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0613d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0613d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0613d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0613d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0613d-137">Response</span></span>
<span data-ttu-id="0613d-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0613d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.relation)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "052c749c-749c-052c-9c74-2c059c742c05",
      "relationship": "pin"
    }
  ]
}
```


[set]: ../resources/termstore-set.md
[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/term list relations",
  "suppressions": [
  ]
}
-->


