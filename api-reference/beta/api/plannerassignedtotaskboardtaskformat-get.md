---
title: Obter plannerAssignedToTaskBoardTaskFormat
description: Recupere as propriedades e as relações do **objeto plannerAssignedToTaskBoardTaskFormat.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 35a4e4fda3fba813873727ab7fa4cf013e610b2c
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473322"
---
# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="46096-103">Obter plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="46096-103">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="46096-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46096-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46096-105">Recupere as propriedades e as relações do **objeto plannerAssignedToTaskBoardTaskFormat.**</span><span class="sxs-lookup"><span data-stu-id="46096-105">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="46096-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46096-106">Permissions</span></span>
<span data-ttu-id="46096-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46096-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46096-109">Permission type</span></span>      | <span data-ttu-id="46096-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46096-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46096-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46096-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46096-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46096-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="46096-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46096-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46096-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46096-114">Not supported.</span></span>    |
|<span data-ttu-id="46096-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46096-115">Application</span></span> | <span data-ttu-id="46096-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46096-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46096-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46096-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="46096-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46096-118">Request headers</span></span>
| <span data-ttu-id="46096-119">Nome</span><span class="sxs-lookup"><span data-stu-id="46096-119">Name</span></span>      |<span data-ttu-id="46096-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="46096-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46096-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="46096-121">Authorization</span></span>  | <span data-ttu-id="46096-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46096-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46096-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46096-124">Request body</span></span>
<span data-ttu-id="46096-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46096-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46096-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="46096-126">Response</span></span>

<span data-ttu-id="46096-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46096-127">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="46096-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="46096-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="46096-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="46096-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="46096-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="46096-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="46096-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46096-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46096-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46096-132">Request</span></span>
<span data-ttu-id="46096-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46096-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46096-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="46096-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="46096-135">C#</span><span class="sxs-lookup"><span data-stu-id="46096-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46096-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46096-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46096-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46096-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46096-138">Java</span><span class="sxs-lookup"><span data-stu-id="46096-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="46096-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="46096-139">Response</span></span>
<span data-ttu-id="46096-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46096-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


