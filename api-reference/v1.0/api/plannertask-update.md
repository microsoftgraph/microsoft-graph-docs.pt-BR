---
title: Atualizar plannertask
description: Atualize as propriedades do **objeto plannertask.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 410913ba71a7b3404169fbfa2e6f06dcaa47038f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722031"
---
# <a name="update-plannertask"></a><span data-ttu-id="2d811-103">Atualizar plannertask</span><span class="sxs-lookup"><span data-stu-id="2d811-103">Update plannertask</span></span>

<span data-ttu-id="2d811-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d811-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d811-105">Atualize as propriedades do **objeto plannertask.**</span><span class="sxs-lookup"><span data-stu-id="2d811-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d811-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2d811-106">Permissions</span></span>
<span data-ttu-id="2d811-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d811-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d811-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d811-109">Permission type</span></span>      | <span data-ttu-id="2d811-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d811-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d811-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d811-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d811-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d811-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d811-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d811-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d811-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d811-114">Not supported.</span></span>    |
|<span data-ttu-id="2d811-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d811-115">Application</span></span> | <span data-ttu-id="2d811-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d811-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d811-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d811-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2d811-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2d811-118">Optional request headers</span></span>
| <span data-ttu-id="2d811-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2d811-119">Name</span></span>       | <span data-ttu-id="2d811-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d811-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2d811-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d811-121">Authorization</span></span>  | <span data-ttu-id="2d811-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d811-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d811-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="2d811-124">If-Match</span></span>  | <span data-ttu-id="2d811-125">Último valor ETag conhecido para o **plannerTask** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="2d811-125">Last known ETag value for the **plannerTask** to be updated.</span></span> <span data-ttu-id="2d811-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d811-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d811-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d811-127">Request body</span></span>
<span data-ttu-id="2d811-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2d811-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d811-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d811-131">Property</span></span>     | <span data-ttu-id="2d811-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d811-132">Type</span></span>   |<span data-ttu-id="2d811-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d811-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d811-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="2d811-134">appliedCategories</span></span>|[<span data-ttu-id="2d811-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="2d811-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="2d811-p105">As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="2d811-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="2d811-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="2d811-138">assigneePriority</span></span>|<span data-ttu-id="2d811-139">String</span><span class="sxs-lookup"><span data-stu-id="2d811-139">String</span></span>|<span data-ttu-id="2d811-140">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="2d811-140">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="2d811-141">O formato é definido em [Usando dicas de ordem no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="2d811-141">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2d811-142">assignments</span><span class="sxs-lookup"><span data-stu-id="2d811-142">assignments</span></span>|[<span data-ttu-id="2d811-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="2d811-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="2d811-144">O conjunto de usuários aos que a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="2d811-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="2d811-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="2d811-145">bucketId</span></span>|<span data-ttu-id="2d811-146">String</span><span class="sxs-lookup"><span data-stu-id="2d811-146">String</span></span>|<span data-ttu-id="2d811-147">ID de bucket à qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="2d811-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="2d811-148">O bucket precisa estar no plano no qual a tarefa está.</span><span class="sxs-lookup"><span data-stu-id="2d811-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="2d811-149">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="2d811-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2d811-150">[Formatar validação](../resources/planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="2d811-150">[Format validation](../resources/planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="2d811-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="2d811-151">conversationThreadId</span></span>|<span data-ttu-id="2d811-152">String</span><span class="sxs-lookup"><span data-stu-id="2d811-152">String</span></span>|<span data-ttu-id="2d811-153">ID de thread da conversa na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2d811-153">Thread id of the conversation on the task.</span></span> <span data-ttu-id="2d811-154">Esta é a id do objeto thread de conversa criado no grupo.</span><span class="sxs-lookup"><span data-stu-id="2d811-154">This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="2d811-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2d811-155">dueDateTime</span></span>|<span data-ttu-id="2d811-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d811-156">DateTimeOffset</span></span>|<span data-ttu-id="2d811-157">Data e hora em que a tarefa é devida.</span><span class="sxs-lookup"><span data-stu-id="2d811-157">Date and time at which the task is due.</span></span> <span data-ttu-id="2d811-158">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2d811-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2d811-159">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2d811-159">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2d811-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="2d811-160">orderHint</span></span>|<span data-ttu-id="2d811-161">String</span><span class="sxs-lookup"><span data-stu-id="2d811-161">String</span></span>|<span data-ttu-id="2d811-162">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="2d811-162">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="2d811-163">O formato é definido em [Usando dicas de ordem no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="2d811-163">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2d811-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="2d811-164">percentComplete</span></span>|<span data-ttu-id="2d811-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2d811-165">Int32</span></span>|<span data-ttu-id="2d811-p111">A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída.</span><span class="sxs-lookup"><span data-stu-id="2d811-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="2d811-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2d811-168">startDateTime</span></span>|<span data-ttu-id="2d811-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d811-169">DateTimeOffset</span></span>|<span data-ttu-id="2d811-170">Data e hora em que a tarefa é iniciada.</span><span class="sxs-lookup"><span data-stu-id="2d811-170">Date and time at which the task starts.</span></span> <span data-ttu-id="2d811-171">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2d811-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2d811-172">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2d811-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2d811-173">title</span><span class="sxs-lookup"><span data-stu-id="2d811-173">title</span></span>|<span data-ttu-id="2d811-174">String</span><span class="sxs-lookup"><span data-stu-id="2d811-174">String</span></span>|<span data-ttu-id="2d811-175">Título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2d811-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="2d811-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d811-176">Response</span></span>

<span data-ttu-id="2d811-177">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [plannerTask](../resources/plannertask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d811-177">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="2d811-p113">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="2d811-p113">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="2d811-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d811-181">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d811-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d811-182">Request</span></span>
<span data-ttu-id="2d811-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d811-183">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d811-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d811-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}
Content-type: application/json
Content-length: 247
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": "N9917 U2883!"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category4": false
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="2d811-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d811-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2d811-186">C#</span><span class="sxs-lookup"><span data-stu-id="2d811-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d811-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d811-187">Response</span></span>
<span data-ttu-id="2d811-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d811-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1423

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
  "createdDateTime": "2015-03-24T18:36:49.2407981Z",
  "assignments": {
    "6463a5ce-2119-4198-9f2a-628761df4a62": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "N9917"
    },
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2017-04-24T22:40:44.5665917",
      "orderHint": "RWk1"
    },
    "aaa27244-1db4-476a-a5cb-004607466324": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "U2883"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category5": true,
    "category6": true,
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

