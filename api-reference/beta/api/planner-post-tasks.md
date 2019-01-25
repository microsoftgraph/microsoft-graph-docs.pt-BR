---
title: Criar plannerTask
description: Use essa API para criar um novo **plannerTask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f74e41e3c855fd6cf54019e2cfd13e36fce45b7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518692"
---
# <a name="create-plannertask"></a><span data-ttu-id="73cdb-103">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="73cdb-103">Create plannerTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73cdb-104">Use essa API para criar um novo **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="73cdb-104">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="73cdb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="73cdb-105">Permissions</span></span>
<span data-ttu-id="73cdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73cdb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73cdb-108">Permission type</span></span>      | <span data-ttu-id="73cdb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73cdb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73cdb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73cdb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73cdb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73cdb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="73cdb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73cdb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73cdb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73cdb-113">Not supported.</span></span>    |
|<span data-ttu-id="73cdb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73cdb-114">Application</span></span> | <span data-ttu-id="73cdb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73cdb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73cdb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73cdb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="73cdb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73cdb-117">Request headers</span></span>
| <span data-ttu-id="73cdb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="73cdb-118">Name</span></span>       | <span data-ttu-id="73cdb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="73cdb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73cdb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="73cdb-120">Authorization</span></span>  | <span data-ttu-id="73cdb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73cdb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73cdb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73cdb-123">Request body</span></span>
<span data-ttu-id="73cdb-p103">No corpo da solicitação, forneça uma representação JSON do objeto [plannerTask](../resources/plannertask.md). A propriedade planId do **plannerTask** deve ser definida como a id de um objeto [plannerPlan](../resources/plannerplan.md) existente.</span><span class="sxs-lookup"><span data-stu-id="73cdb-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="73cdb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="73cdb-126">Response</span></span>

<span data-ttu-id="73cdb-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73cdb-127">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="73cdb-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="73cdb-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="73cdb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73cdb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73cdb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73cdb-132">Request</span></span>
<span data-ttu-id="73cdb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73cdb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  },
}
```
<span data-ttu-id="73cdb-134">No corpo da solicitação, forneça uma representação JSON do objeto [plannerTask](../resources/plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="73cdb-134">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="73cdb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="73cdb-135">Response</span></span>
<span data-ttu-id="73cdb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73cdb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
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
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planner-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
