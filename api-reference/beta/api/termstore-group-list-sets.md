---
title: Listar conjuntos
description: Obter uma lista dos objetos set e suas propriedades.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4d358769f7d4a73c2f01f84e0237747c456307a5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873938"
---
# <a name="list-sets"></a><span data-ttu-id="1d34f-103">Listar conjuntos</span><span class="sxs-lookup"><span data-stu-id="1d34f-103">List sets</span></span>
<span data-ttu-id="1d34f-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="1d34f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d34f-105">Obter uma lista dos [objetos set](../resources/termstore-set.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1d34f-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d34f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d34f-106">Permissions</span></span>
<span data-ttu-id="1d34f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d34f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d34f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d34f-109">Permission type</span></span>|<span data-ttu-id="1d34f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d34f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d34f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d34f-111">Delegated (work or school account)</span></span> |<span data-ttu-id="1d34f-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d34f-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="1d34f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d34f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d34f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d34f-114">Not supported.</span></span>    |
|<span data-ttu-id="1d34f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d34f-115">Application</span></span> | <span data-ttu-id="1d34f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d34f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d34f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d34f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d34f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d34f-118">Optional query parameters</span></span>
<span data-ttu-id="1d34f-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d34f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1d34f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1d34f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d34f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d34f-121">Request headers</span></span>
|<span data-ttu-id="1d34f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1d34f-122">Name</span></span>|<span data-ttu-id="1d34f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d34f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d34f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d34f-124">Authorization</span></span>|<span data-ttu-id="1d34f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d34f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d34f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d34f-127">Request body</span></span>
<span data-ttu-id="1d34f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d34f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d34f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d34f-129">Response</span></span>

<span data-ttu-id="1d34f-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos definidos](../resources/termstore-set.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d34f-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d34f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d34f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d34f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d34f-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1d34f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d34f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="1d34f-134">C#</span><span class="sxs-lookup"><span data-stu-id="1d34f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d34f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d34f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d34f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d34f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d34f-137">Java</span><span class="sxs-lookup"><span data-stu-id="1d34f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1d34f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d34f-138">Response</span></span>

<span data-ttu-id="1d34f-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d34f-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


