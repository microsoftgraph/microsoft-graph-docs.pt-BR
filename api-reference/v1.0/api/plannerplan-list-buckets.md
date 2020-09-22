---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket** contidos em um objeto plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 88d6156b35063ccb5454278d38505c4f4dbd6291
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020657"
---
# <a name="list-buckets"></a><span data-ttu-id="e419b-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="e419b-103">List buckets</span></span>

<span data-ttu-id="e419b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e419b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e419b-105">Recupere uma lista de objetos [plannerBucket](../resources/plannerbucket.md) contidos em um objeto [plannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="e419b-105">Retrieve a list of [plannerBucket](../resources/plannerbucket.md) objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e419b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e419b-106">Permissions</span></span>
<span data-ttu-id="e419b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e419b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e419b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e419b-109">Permission type</span></span>      | <span data-ttu-id="e419b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e419b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e419b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e419b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e419b-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e419b-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e419b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e419b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e419b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e419b-114">Not supported.</span></span>    |
|<span data-ttu-id="e419b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e419b-115">Application</span></span> | <span data-ttu-id="e419b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e419b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e419b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e419b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="e419b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e419b-118">Request headers</span></span>
| <span data-ttu-id="e419b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e419b-119">Name</span></span>      |<span data-ttu-id="e419b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e419b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e419b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e419b-121">Authorization</span></span>  | <span data-ttu-id="e419b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e419b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e419b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e419b-124">Request body</span></span>
<span data-ttu-id="e419b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e419b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e419b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e419b-126">Response</span></span>

<span data-ttu-id="e419b-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e419b-127">If successful, this method returns a `200 OK` response code and a collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="e419b-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="e419b-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="e419b-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="e419b-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="e419b-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e419b-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="e419b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e419b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e419b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e419b-132">Request</span></span>
<span data-ttu-id="e419b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e419b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e419b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e419b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
# <a name="c"></a>[<span data-ttu-id="e419b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e419b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e419b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e419b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e419b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e419b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e419b-138">Java</span><span class="sxs-lookup"><span data-stu-id="e419b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e419b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e419b-139">Response</span></span>
<span data-ttu-id="e419b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e419b-140">Here is an example of the response.</span></span> 

><span data-ttu-id="e419b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e419b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

