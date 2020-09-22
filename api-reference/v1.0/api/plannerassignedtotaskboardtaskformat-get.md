---
title: Obter plannerAssignedToTaskBoardTaskFormat
description: Recupere as propriedades e os relacionamentos do objeto **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 08c41531ec40b510813b9c324139fccc7948f018
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025617"
---
# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="b39a3-103">Obter plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b39a3-103">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="b39a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b39a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b39a3-105">Recupere as propriedades e os relacionamentos do objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="b39a3-105">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b39a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b39a3-106">Permissions</span></span>
<span data-ttu-id="b39a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b39a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b39a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b39a3-109">Permission type</span></span>      | <span data-ttu-id="b39a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b39a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b39a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b39a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b39a3-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b39a3-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b39a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b39a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b39a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b39a3-114">Not supported.</span></span>    |
|<span data-ttu-id="b39a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b39a3-115">Application</span></span> | <span data-ttu-id="b39a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b39a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b39a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b39a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="b39a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b39a3-118">Request headers</span></span>
| <span data-ttu-id="b39a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b39a3-119">Name</span></span>      |<span data-ttu-id="b39a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39a3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b39a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b39a3-121">Authorization</span></span>  | <span data-ttu-id="b39a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b39a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b39a3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b39a3-124">Request body</span></span>
<span data-ttu-id="b39a3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b39a3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b39a3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b39a3-126">Response</span></span>

<span data-ttu-id="b39a3-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b39a3-127">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="b39a3-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="b39a3-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="b39a3-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="b39a3-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="b39a3-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b39a3-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b39a3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b39a3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b39a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b39a3-132">Request</span></span>
<span data-ttu-id="b39a3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b39a3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b39a3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b39a3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="b39a3-135">C#</span><span class="sxs-lookup"><span data-stu-id="b39a3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b39a3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b39a3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b39a3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b39a3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b39a3-138">Java</span><span class="sxs-lookup"><span data-stu-id="b39a3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b39a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b39a3-139">Response</span></span>
<span data-ttu-id="b39a3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b39a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

