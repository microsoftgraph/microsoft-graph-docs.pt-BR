---
title: Listar tarefas
description: Recupere uma lista de objetos **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8011976b880cc4cbcc3645ed9bbacb67a97be806
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524734"
---
# <a name="list-tasks"></a><span data-ttu-id="d52bd-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d52bd-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d52bd-104">Recupere uma lista de objetos **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="d52bd-104">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d52bd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d52bd-105">Permissions</span></span>
<span data-ttu-id="d52bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d52bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d52bd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d52bd-108">Permission type</span></span>      | <span data-ttu-id="d52bd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d52bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d52bd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d52bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d52bd-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52bd-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d52bd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d52bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d52bd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d52bd-113">Not supported.</span></span>    |
|<span data-ttu-id="d52bd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d52bd-114">Application</span></span> | <span data-ttu-id="d52bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d52bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d52bd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d52bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d52bd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d52bd-117">Optional query parameters</span></span>
<span data-ttu-id="d52bd-118">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de planId seja especificado.</span><span class="sxs-lookup"><span data-stu-id="d52bd-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d52bd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d52bd-119">Request headers</span></span>
| <span data-ttu-id="d52bd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d52bd-120">Name</span></span>      |<span data-ttu-id="d52bd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d52bd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d52bd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d52bd-122">Authorization</span></span>  | <span data-ttu-id="d52bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d52bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d52bd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d52bd-125">Request body</span></span>
<span data-ttu-id="d52bd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d52bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d52bd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d52bd-127">Response</span></span>

<span data-ttu-id="d52bd-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d52bd-128">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="d52bd-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d52bd-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="d52bd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d52bd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d52bd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d52bd-133">Request</span></span>
<span data-ttu-id="d52bd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d52bd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks
```
##### <a name="response"></a><span data-ttu-id="d52bd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d52bd-135">Response</span></span>
<span data-ttu-id="d52bd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d52bd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/planner-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
