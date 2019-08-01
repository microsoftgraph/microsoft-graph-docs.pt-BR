---
title: Listar buckets
description: Recupere uma lista de objetos **plannerbucket** contidos em um objeto plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1218da89e212de480bd18084af37f5af534b82bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976107"
---
# <a name="list-buckets"></a><span data-ttu-id="c54e7-103">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="c54e7-103">List buckets</span></span>

<span data-ttu-id="c54e7-104">Recupere uma lista de objetos [plannerBucket](../resources/plannerbucket.md) contidos em um objeto [plannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="c54e7-104">Retrieve a list of [plannerBucket](../resources/plannerbucket.md) objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c54e7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c54e7-105">Permissions</span></span>
<span data-ttu-id="c54e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54e7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c54e7-108">Permission type</span></span>      | <span data-ttu-id="c54e7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c54e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c54e7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c54e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c54e7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c54e7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c54e7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c54e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c54e7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c54e7-113">Not supported.</span></span>    |
|<span data-ttu-id="c54e7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c54e7-114">Application</span></span> | <span data-ttu-id="c54e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c54e7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c54e7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c54e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="c54e7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c54e7-117">Request headers</span></span>
| <span data-ttu-id="c54e7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c54e7-118">Name</span></span>      |<span data-ttu-id="c54e7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54e7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c54e7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c54e7-120">Authorization</span></span>  | <span data-ttu-id="c54e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c54e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c54e7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c54e7-123">Request body</span></span>
<span data-ttu-id="c54e7-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c54e7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c54e7-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54e7-125">Response</span></span>

<span data-ttu-id="c54e7-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54e7-126">If successful, this method returns a `200 OK` response code and a collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="c54e7-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="c54e7-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="c54e7-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="c54e7-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="c54e7-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c54e7-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="c54e7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c54e7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c54e7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54e7-131">Request</span></span>
<span data-ttu-id="c54e7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c54e7-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c54e7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54e7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c54e7-134">C#</span><span class="sxs-lookup"><span data-stu-id="c54e7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c54e7-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c54e7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c54e7-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c54e7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c54e7-137">Java</span><span class="sxs-lookup"><span data-stu-id="c54e7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54e7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54e7-138">Response</span></span>
<span data-ttu-id="c54e7-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54e7-139">Here is an example of the response.</span></span> 

><span data-ttu-id="c54e7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c54e7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
