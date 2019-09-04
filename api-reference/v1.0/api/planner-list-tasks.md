---
title: Listar tarefas
description: Recupere uma lista de objetos **plannertask** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: d8692c0f1ec35c449b0803dd8c6f73fda3d89cbc
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730040"
---
# <a name="list-tasks"></a><span data-ttu-id="7bdb3-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="7bdb3-103">List tasks</span></span>

<span data-ttu-id="7bdb3-104">Recupere uma lista de objetos **plannertask** .</span><span class="sxs-lookup"><span data-stu-id="7bdb3-104">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7bdb3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bdb3-105">Permissions</span></span>
<span data-ttu-id="7bdb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bdb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bdb3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bdb3-108">Permission type</span></span>      | <span data-ttu-id="7bdb3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bdb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bdb3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bdb3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7bdb3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bdb3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bdb3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bdb3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bdb3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-113">Not supported.</span></span>    |
|<span data-ttu-id="7bdb3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bdb3-114">Application</span></span> | <span data-ttu-id="7bdb3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bdb3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bdb3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7bdb3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7bdb3-117">Optional query parameters</span></span>
<span data-ttu-id="7bdb3-118">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de PlanID seja especificado.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bdb3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bdb3-119">Request headers</span></span>
| <span data-ttu-id="7bdb3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7bdb3-120">Name</span></span>      |<span data-ttu-id="7bdb3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bdb3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bdb3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bdb3-122">Authorization</span></span>  | <span data-ttu-id="7bdb3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bdb3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bdb3-125">Request body</span></span>
<span data-ttu-id="7bdb3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bdb3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bdb3-127">Response</span></span>

<span data-ttu-id="7bdb3-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-128">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="7bdb3-129">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="7bdb3-129">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="7bdb3-130">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-130">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="7bdb3-131">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7bdb3-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="7bdb3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bdb3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bdb3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bdb3-133">Request</span></span>
<span data-ttu-id="7bdb3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7bdb3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bdb3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bdb3-136">C#</span><span class="sxs-lookup"><span data-stu-id="7bdb3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bdb3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bdb3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bdb3-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bdb3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bdb3-139">Java</span><span class="sxs-lookup"><span data-stu-id="7bdb3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7bdb3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bdb3-140">Response</span></span>
<span data-ttu-id="7bdb3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bdb3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
