---
title: Listar conjuntos
description: Obtenha uma lista dos objetos Set e suas propriedades.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 951a1e0522695a81061142dc7f76639ed4bb353c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092962"
---
# <a name="list-sets"></a><span data-ttu-id="d2835-103">Listar conjuntos</span><span class="sxs-lookup"><span data-stu-id="d2835-103">List sets</span></span>
<span data-ttu-id="d2835-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="d2835-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2835-105">Obtenha uma lista dos objetos [set](../resources/termstore-set.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d2835-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2835-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2835-106">Permissions</span></span>
<span data-ttu-id="d2835-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2835-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2835-109">Permission type</span></span>|<span data-ttu-id="d2835-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2835-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2835-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2835-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d2835-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2835-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d2835-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2835-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2835-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2835-114">Not supported.</span></span>    |
|<span data-ttu-id="d2835-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2835-115">Application</span></span> | <span data-ttu-id="d2835-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2835-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2835-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2835-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2835-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2835-118">Optional query parameters</span></span>
<span data-ttu-id="d2835-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2835-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d2835-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d2835-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2835-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2835-121">Request headers</span></span>
|<span data-ttu-id="d2835-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d2835-122">Name</span></span>|<span data-ttu-id="d2835-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2835-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2835-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2835-124">Authorization</span></span>|<span data-ttu-id="d2835-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2835-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2835-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2835-127">Request body</span></span>
<span data-ttu-id="d2835-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2835-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2835-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2835-129">Response</span></span>

<span data-ttu-id="d2835-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [set](../resources/termstore-set.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2835-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2835-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2835-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2835-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2835-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d2835-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2835-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="d2835-134">C#</span><span class="sxs-lookup"><span data-stu-id="d2835-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2835-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2835-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2835-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2835-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d2835-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2835-137">Response</span></span>

<span data-ttu-id="d2835-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d2835-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.set)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
      "description": "Starting term Set",    
      "localizedNames" : [
        {
          "languageTag" : "en-US",
          "name" : "Department"
        }
      ]
    }
  ]
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termstore-set",
  "suppressions": [
  ]
}
-->


