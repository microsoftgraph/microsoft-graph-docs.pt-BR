---
title: Listar grupos
description: Obter os grupos da propriedade de navegação grupos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3996bf2cc502f47ad5a2ce60fc92bd9f9d570fe1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957153"
---
# <a name="list-groups"></a><span data-ttu-id="f15e7-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="f15e7-103">List groups</span></span>
<span data-ttu-id="f15e7-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="f15e7-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f15e7-105">Obter a lista de [objetos de](../resources/termstore-group.md) grupo de um [armazenamento](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="f15e7-105">Get the list of [group](../resources/termstore-group.md) objects of a [store](../resources/termstore-store.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="f15e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f15e7-106">Permissions</span></span>
<span data-ttu-id="f15e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f15e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f15e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f15e7-109">Permission type</span></span>|<span data-ttu-id="f15e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f15e7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f15e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f15e7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f15e7-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15e7-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f15e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f15e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f15e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f15e7-114">Not supported.</span></span>    |
|<span data-ttu-id="f15e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f15e7-115">Application</span></span> | <span data-ttu-id="f15e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f15e7-116">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f15e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f15e7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f15e7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f15e7-118">Optional query parameters</span></span>
<span data-ttu-id="f15e7-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f15e7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f15e7-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f15e7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f15e7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f15e7-121">Request headers</span></span>
|<span data-ttu-id="f15e7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f15e7-122">Name</span></span>|<span data-ttu-id="f15e7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f15e7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f15e7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f15e7-124">Authorization</span></span>|<span data-ttu-id="f15e7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f15e7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f15e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f15e7-127">Request body</span></span>
<span data-ttu-id="f15e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f15e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f15e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f15e7-129">Response</span></span>

<span data-ttu-id="f15e7-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/termstore-group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f15e7-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/termstore-group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f15e7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f15e7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f15e7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f15e7-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f15e7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f15e7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups
```
# <a name="c"></a>[<span data-ttu-id="f15e7-134">C#</span><span class="sxs-lookup"><span data-stu-id="f15e7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f15e7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f15e7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f15e7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f15e7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f15e7-137">Java</span><span class="sxs-lookup"><span data-stu-id="f15e7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f15e7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f15e7-138">Response</span></span>
<span data-ttu-id="f15e7-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f15e7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.group)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "85825593-5593-8582-9355-828593558285",
      "createdDateTime": "2019-06-21T20:01:37Z",
      "description": "My term group",
      "scope" : "global",
      "displayName": "myGroup"  
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termGroups",
  "suppressions": [
  ]
}
-->



