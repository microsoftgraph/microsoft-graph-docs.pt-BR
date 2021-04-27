---
title: Listar tarefas
description: Recupere uma lista de objetos **plannertask** atribuídos a um Usuário.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 70cc0b8f59b5907b98a42c5b6a00f1b1e09ed50f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049930"
---
# <a name="list-tasks"></a><span data-ttu-id="27baa-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="27baa-103">List tasks</span></span>

<span data-ttu-id="27baa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27baa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27baa-105">Recupere uma lista de objetos **plannertask** atribuídos a um Usuário.</span><span class="sxs-lookup"><span data-stu-id="27baa-105">Retrieve a list of **plannertask** objects assigned to a User.</span></span>

## <a name="permissions"></a><span data-ttu-id="27baa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="27baa-106">Permissions</span></span>
<span data-ttu-id="27baa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27baa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27baa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27baa-109">Permission type</span></span>      | <span data-ttu-id="27baa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27baa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27baa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27baa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="27baa-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27baa-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="27baa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27baa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27baa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27baa-114">Not supported.</span></span>    |
|<span data-ttu-id="27baa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27baa-115">Application</span></span> | <span data-ttu-id="27baa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27baa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27baa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27baa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/tasks
GET /users/{id}/planner/tasks
```

## <a name="request-headers"></a><span data-ttu-id="27baa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27baa-118">Request headers</span></span>
| <span data-ttu-id="27baa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="27baa-119">Name</span></span>      |<span data-ttu-id="27baa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27baa-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27baa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="27baa-121">Authorization</span></span>  | <span data-ttu-id="27baa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27baa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27baa-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27baa-124">Request body</span></span>
<span data-ttu-id="27baa-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27baa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27baa-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="27baa-126">Response</span></span>

<span data-ttu-id="27baa-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27baa-127">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="27baa-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="27baa-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="27baa-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="27baa-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="27baa-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="27baa-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="27baa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27baa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27baa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27baa-132">Request</span></span>
<span data-ttu-id="27baa-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27baa-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27baa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="27baa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "planneruser_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/tasks
```
# <a name="c"></a>[<span data-ttu-id="27baa-135">C#</span><span class="sxs-lookup"><span data-stu-id="27baa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/planneruser-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27baa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27baa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/planneruser-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27baa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27baa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/planneruser-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27baa-138">Java</span><span class="sxs-lookup"><span data-stu-id="27baa-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/planneruser-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27baa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="27baa-139">Response</span></span>
<span data-ttu-id="27baa-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27baa-140">Here is an example of the response.</span></span> <span data-ttu-id="27baa-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27baa-141">Note: The response object shown here might be shortened for readability.</span></span>
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


