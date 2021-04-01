---
title: Obter plannerTask
description: Recupere as propriedades e as relações do **objeto plannertask.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 85810854b40f8fafb828bd59c9317dd44d57924d
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473497"
---
# <a name="get-plannertask"></a><span data-ttu-id="a9331-103">Obter plannerTask</span><span class="sxs-lookup"><span data-stu-id="a9331-103">Get plannerTask</span></span>

<span data-ttu-id="a9331-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9331-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9331-105">Recupere as propriedades e as relações do **objeto plannertask.**</span><span class="sxs-lookup"><span data-stu-id="a9331-105">Retrieve the properties and relationships of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9331-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9331-106">Permissions</span></span>
<span data-ttu-id="a9331-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9331-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9331-109">Permission type</span></span>      | <span data-ttu-id="a9331-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9331-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9331-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9331-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9331-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9331-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9331-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9331-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9331-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9331-114">Not supported.</span></span>    |
|<span data-ttu-id="a9331-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9331-115">Application</span></span> | <span data-ttu-id="a9331-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9331-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9331-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9331-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9331-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9331-118">Request headers</span></span>
| <span data-ttu-id="a9331-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a9331-119">Name</span></span>      |<span data-ttu-id="a9331-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9331-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9331-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9331-121">Authorization</span></span>  | <span data-ttu-id="a9331-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9331-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9331-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9331-124">Request body</span></span>
<span data-ttu-id="a9331-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9331-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9331-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9331-126">Response</span></span>

<span data-ttu-id="a9331-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9331-127">If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="a9331-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="a9331-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="a9331-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="a9331-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="a9331-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a9331-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a9331-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9331-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9331-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9331-132">Request</span></span>
<span data-ttu-id="a9331-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9331-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9331-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9331-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
```
# <a name="c"></a>[<span data-ttu-id="a9331-135">C#</span><span class="sxs-lookup"><span data-stu-id="a9331-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9331-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9331-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9331-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9331-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9331-138">Java</span><span class="sxs-lookup"><span data-stu-id="a9331-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannertask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9331-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9331-139">Response</span></span>
<span data-ttu-id="a9331-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9331-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 707

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


