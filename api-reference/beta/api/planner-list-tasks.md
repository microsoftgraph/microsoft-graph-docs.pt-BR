---
title: Listar tarefas
description: Recupere uma lista de objetos **plannertask.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 15b27dce703c8e8e23742252584181d35911ce69
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055362"
---
# <a name="list-tasks"></a><span data-ttu-id="7de83-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="7de83-103">List tasks</span></span>

<span data-ttu-id="7de83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de83-105">Recupere uma lista de objetos **plannertask.**</span><span class="sxs-lookup"><span data-stu-id="7de83-105">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7de83-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7de83-106">Permissions</span></span>
<span data-ttu-id="7de83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7de83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7de83-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7de83-109">Permission type</span></span>      | <span data-ttu-id="7de83-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7de83-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7de83-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7de83-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7de83-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7de83-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7de83-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7de83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7de83-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7de83-114">Not supported.</span></span>    |
|<span data-ttu-id="7de83-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7de83-115">Application</span></span> | <span data-ttu-id="7de83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7de83-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7de83-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7de83-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7de83-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7de83-118">Optional query parameters</span></span>
<span data-ttu-id="7de83-119">Este método exige [que](/graph/query-parameters) o filtro planId seja especificado.</span><span class="sxs-lookup"><span data-stu-id="7de83-119">This method requires planId [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7de83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7de83-120">Request headers</span></span>
| <span data-ttu-id="7de83-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7de83-121">Name</span></span>      |<span data-ttu-id="7de83-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7de83-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7de83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7de83-123">Authorization</span></span>  | <span data-ttu-id="7de83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7de83-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7de83-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7de83-126">Request body</span></span>
<span data-ttu-id="7de83-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7de83-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7de83-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de83-128">Response</span></span>

<span data-ttu-id="7de83-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7de83-129">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="7de83-130">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="7de83-130">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="7de83-131">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="7de83-131">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="7de83-132">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7de83-132">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="7de83-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7de83-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7de83-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7de83-134">Request</span></span>
<span data-ttu-id="7de83-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7de83-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7de83-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7de83-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "planner_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks
```
# <a name="c"></a>[<span data-ttu-id="7de83-137">C#</span><span class="sxs-lookup"><span data-stu-id="7de83-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/planner-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7de83-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7de83-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/planner-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7de83-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7de83-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/planner-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7de83-140">Java</span><span class="sxs-lookup"><span data-stu-id="7de83-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/planner-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7de83-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de83-141">Response</span></span>
<span data-ttu-id="7de83-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7de83-142">Here is an example of the response.</span></span> <span data-ttu-id="7de83-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7de83-143">Note: The response object shown here might be shortened for readability.</span></span>
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
