---
title: Listar grupos
description: Obtenha os grupos da propriedade de navegação grupos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: c1225bf6f9aacef77ece20c659a51b36d362ff31
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329340"
---
# <a name="list-groups"></a><span data-ttu-id="7aff3-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="7aff3-103">List groups</span></span>
<span data-ttu-id="7aff3-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="7aff3-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aff3-105">Obter a lista de objetos de [grupo](../resources/termstore-group.md) de um [repositório](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="7aff3-105">Get the list of [group](../resources/termstore-group.md) objects of a [store](../resources/termstore-store.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="7aff3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aff3-106">Permissions</span></span>
<span data-ttu-id="7aff3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aff3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aff3-109">Permission type</span></span>|<span data-ttu-id="7aff3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7aff3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aff3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aff3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7aff3-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7aff3-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="7aff3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aff3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aff3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aff3-114">Not supported.</span></span>    |
|<span data-ttu-id="7aff3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aff3-115">Application</span></span> | <span data-ttu-id="7aff3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aff3-116">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aff3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aff3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7aff3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7aff3-118">Optional query parameters</span></span>
<span data-ttu-id="7aff3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7aff3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7aff3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7aff3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aff3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aff3-121">Request headers</span></span>
|<span data-ttu-id="7aff3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7aff3-122">Name</span></span>|<span data-ttu-id="7aff3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aff3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7aff3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aff3-124">Authorization</span></span>|<span data-ttu-id="7aff3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aff3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aff3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aff3-127">Request body</span></span>
<span data-ttu-id="7aff3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7aff3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aff3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aff3-129">Response</span></span>

<span data-ttu-id="7aff3-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aff3-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/termstore-group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7aff3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7aff3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7aff3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aff3-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7aff3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aff3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups
```
# <a name="c"></a>[<span data-ttu-id="7aff3-134">C#</span><span class="sxs-lookup"><span data-stu-id="7aff3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7aff3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aff3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7aff3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aff3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7aff3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aff3-137">Response</span></span>
<span data-ttu-id="7aff3-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7aff3-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

