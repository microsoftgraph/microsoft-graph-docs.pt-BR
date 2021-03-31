---
title: Listar tarefas
description: Recupere uma lista de objetos **plannerTask** associados a um objeto plannerBucket.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 57413c3b1bf58699c505984413d01bf8ec563f2e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473172"
---
# <a name="list-tasks"></a><span data-ttu-id="1b5b4-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="1b5b4-103">List tasks</span></span>

<span data-ttu-id="1b5b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b5b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b5b4-105">Recupere uma lista de objetos **plannerTask** associados a um [objeto plannerBucket.](../resources/plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="1b5b4-105">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerbucket.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b5b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b5b4-106">Permissions</span></span>
<span data-ttu-id="1b5b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b5b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b5b4-109">Permission type</span></span>      | <span data-ttu-id="1b5b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b5b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b5b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5b4-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5b4-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b5b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b5b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-114">Not supported.</span></span>    |
|<span data-ttu-id="1b5b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b5b4-115">Application</span></span> | <span data-ttu-id="1b5b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b5b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="1b5b4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5b4-118">Request headers</span></span>
| <span data-ttu-id="1b5b4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1b5b4-119">Name</span></span>      |<span data-ttu-id="1b5b4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b5b4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b5b4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b5b4-121">Authorization</span></span>  | <span data-ttu-id="1b5b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b5b4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5b4-124">Request body</span></span>
<span data-ttu-id="1b5b4-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b5b4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5b4-126">Response</span></span>

<span data-ttu-id="1b5b4-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-127">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="1b5b4-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="1b5b4-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="1b5b4-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="1b5b4-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="1b5b4-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="1b5b4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b5b4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b5b4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5b4-132">Request</span></span>
<span data-ttu-id="1b5b4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b5b4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5b4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "plannerbucket_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks
```
# <a name="c"></a>[<span data-ttu-id="1b5b4-135">C#</span><span class="sxs-lookup"><span data-stu-id="1b5b4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/plannerbucket-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b5b4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b5b4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/plannerbucket-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b5b4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b5b4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/plannerbucket-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b5b4-138">Java</span><span class="sxs-lookup"><span data-stu-id="1b5b4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/plannerbucket-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b5b4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5b4-139">Response</span></span>
<span data-ttu-id="1b5b4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b5b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
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
          "@odata.type": "#microsoft.graph.plannerassignment",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


