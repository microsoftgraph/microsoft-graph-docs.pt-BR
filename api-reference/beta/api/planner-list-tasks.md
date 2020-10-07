---
title: Listar tarefas
description: Recupere uma lista de objetos **plannertask** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: dd74b30c91991191df139731fbf5807a14b024db
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373381"
---
# <a name="list-tasks"></a><span data-ttu-id="f6ad6-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="f6ad6-103">List tasks</span></span>

<span data-ttu-id="f6ad6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6ad6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6ad6-105">Recupere uma lista de objetos **plannertask** .</span><span class="sxs-lookup"><span data-stu-id="f6ad6-105">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6ad6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6ad6-106">Permissions</span></span>
<span data-ttu-id="f6ad6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ad6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6ad6-109">Permission type</span></span>      | <span data-ttu-id="f6ad6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6ad6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6ad6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6ad6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6ad6-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ad6-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6ad6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6ad6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6ad6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-114">Not supported.</span></span>    |
|<span data-ttu-id="f6ad6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6ad6-115">Application</span></span> | <span data-ttu-id="f6ad6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6ad6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ad6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6ad6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6ad6-118">Optional query parameters</span></span>
<span data-ttu-id="f6ad6-119">Este método requer que o [filtro](/graph/query-parameters) de PlanID seja especificado.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-119">This method requires planId [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6ad6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6ad6-120">Request headers</span></span>
| <span data-ttu-id="f6ad6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f6ad6-121">Name</span></span>      |<span data-ttu-id="f6ad6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ad6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6ad6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6ad6-123">Authorization</span></span>  | <span data-ttu-id="f6ad6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6ad6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6ad6-126">Request body</span></span>
<span data-ttu-id="f6ad6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ad6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6ad6-128">Response</span></span>

<span data-ttu-id="f6ad6-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-129">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="f6ad6-130">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="f6ad6-130">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="f6ad6-131">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-131">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="f6ad6-132">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f6ad6-132">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="f6ad6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6ad6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6ad6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6ad6-134">Request</span></span>
<span data-ttu-id="f6ad6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6ad6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ad6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "planner_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks
```
# <a name="c"></a>[<span data-ttu-id="f6ad6-137">C#</span><span class="sxs-lookup"><span data-stu-id="f6ad6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/planner-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6ad6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6ad6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/planner-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6ad6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6ad6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/planner-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6ad6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6ad6-140">Response</span></span>
<span data-ttu-id="f6ad6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6ad6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
