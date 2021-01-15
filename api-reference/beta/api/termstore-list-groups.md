---
title: Listar grupos
description: Obter os grupos da propriedade de navegação de grupos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2ee12f8ebc6fe5a6c300af6cfa231ee506fa38f5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873287"
---
# <a name="list-groups"></a><span data-ttu-id="a4fa9-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="a4fa9-103">List groups</span></span>
<span data-ttu-id="a4fa9-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="a4fa9-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4fa9-105">Obter a lista de [objetos de](../resources/termstore-group.md) grupo de um [armazenamento](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="a4fa9-105">Get the list of [group](../resources/termstore-group.md) objects of a [store](../resources/termstore-store.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="a4fa9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4fa9-106">Permissions</span></span>
<span data-ttu-id="a4fa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4fa9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4fa9-109">Permission type</span></span>|<span data-ttu-id="a4fa9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4fa9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4fa9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4fa9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4fa9-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4fa9-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="a4fa9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4fa9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4fa9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-114">Not supported.</span></span>    |
|<span data-ttu-id="a4fa9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4fa9-115">Application</span></span> | <span data-ttu-id="a4fa9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-116">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4fa9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4fa9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4fa9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4fa9-118">Optional query parameters</span></span>
<span data-ttu-id="a4fa9-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a4fa9-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a4fa9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4fa9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4fa9-121">Request headers</span></span>
|<span data-ttu-id="a4fa9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a4fa9-122">Name</span></span>|<span data-ttu-id="a4fa9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4fa9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4fa9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4fa9-124">Authorization</span></span>|<span data-ttu-id="a4fa9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4fa9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4fa9-127">Request body</span></span>
<span data-ttu-id="a4fa9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4fa9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4fa9-129">Response</span></span>

<span data-ttu-id="a4fa9-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de objetos [de](../resources/termstore-group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/termstore-group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4fa9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4fa9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4fa9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4fa9-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4fa9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4fa9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups
```
# <a name="c"></a>[<span data-ttu-id="a4fa9-134">C#</span><span class="sxs-lookup"><span data-stu-id="a4fa9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4fa9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4fa9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4fa9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4fa9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4fa9-137">Java</span><span class="sxs-lookup"><span data-stu-id="a4fa9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a4fa9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4fa9-138">Response</span></span>
<span data-ttu-id="a4fa9-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4fa9-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



