---
title: Atualizar plannertask
description: Atualize as propriedades do **objeto plannertask.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 86e30d8a2d783134c3e32110703348a3014cc208
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048677"
---
# <a name="update-plannertask"></a><span data-ttu-id="ebc6a-103">Atualizar plannertask</span><span class="sxs-lookup"><span data-stu-id="ebc6a-103">Update plannertask</span></span>

<span data-ttu-id="ebc6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebc6a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebc6a-105">Atualize as propriedades do **objeto plannertask.**</span><span class="sxs-lookup"><span data-stu-id="ebc6a-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebc6a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebc6a-106">Permissions</span></span>
<span data-ttu-id="ebc6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebc6a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebc6a-109">Permission type</span></span>      | <span data-ttu-id="ebc6a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebc6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebc6a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebc6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebc6a-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebc6a-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ebc6a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebc6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebc6a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-114">Not supported.</span></span>    |
|<span data-ttu-id="ebc6a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc6a-115">Application</span></span> | <span data-ttu-id="ebc6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebc6a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ebc6a-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ebc6a-118">Optional request headers</span></span>
| <span data-ttu-id="ebc6a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ebc6a-119">Name</span></span>       | <span data-ttu-id="ebc6a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebc6a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ebc6a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebc6a-121">Authorization</span></span>  | <span data-ttu-id="ebc6a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebc6a-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="ebc6a-124">If-Match</span></span>  | <span data-ttu-id="ebc6a-125">Último valor ETag conhecido para o **plannerTask** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-125">Last known ETag value for the **plannerTask** to be updated.</span></span> <span data-ttu-id="ebc6a-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebc6a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc6a-127">Request body</span></span>
<span data-ttu-id="ebc6a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ebc6a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebc6a-131">Property</span></span>     | <span data-ttu-id="ebc6a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebc6a-132">Type</span></span>   |<span data-ttu-id="ebc6a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebc6a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebc6a-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="ebc6a-134">appliedCategories</span></span>|[<span data-ttu-id="ebc6a-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="ebc6a-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="ebc6a-p105">As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="ebc6a-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="ebc6a-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="ebc6a-138">assigneePriority</span></span>|<span data-ttu-id="ebc6a-139">String</span><span class="sxs-lookup"><span data-stu-id="ebc6a-139">String</span></span>|<span data-ttu-id="ebc6a-140">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-140">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="ebc6a-141">O formato é definido em [Usando dicas de ordem no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ebc6a-141">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ebc6a-142">assignments</span><span class="sxs-lookup"><span data-stu-id="ebc6a-142">assignments</span></span>|[<span data-ttu-id="ebc6a-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="ebc6a-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="ebc6a-144">O conjunto de usuários aos que a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="ebc6a-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="ebc6a-145">bucketId</span></span>|<span data-ttu-id="ebc6a-146">String</span><span class="sxs-lookup"><span data-stu-id="ebc6a-146">String</span></span>|<span data-ttu-id="ebc6a-147">ID de bucket à qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="ebc6a-148">O bucket precisa estar no plano no qual a tarefa está.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="ebc6a-149">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ebc6a-150">[Formatar validação](../resources/planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-150">[Format validation](../resources/planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="ebc6a-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="ebc6a-151">conversationThreadId</span></span>|<span data-ttu-id="ebc6a-152">String</span><span class="sxs-lookup"><span data-stu-id="ebc6a-152">String</span></span>|<span data-ttu-id="ebc6a-153">ID de thread da conversa na tarefa.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-153">Thread id of the conversation on the task.</span></span> <span data-ttu-id="ebc6a-154">Esta é a id do objeto thread de conversa criado no grupo.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-154">This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="ebc6a-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="ebc6a-155">dueDateTime</span></span>|<span data-ttu-id="ebc6a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc6a-156">DateTimeOffset</span></span>|<span data-ttu-id="ebc6a-157">A data e a hora que a tarefa já deve estar concluída.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-157">Date and time at which the task is due.</span></span> <span data-ttu-id="ebc6a-158">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ebc6a-159">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ebc6a-159">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ebc6a-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="ebc6a-160">orderHint</span></span>|<span data-ttu-id="ebc6a-161">String</span><span class="sxs-lookup"><span data-stu-id="ebc6a-161">String</span></span>|<span data-ttu-id="ebc6a-162">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-162">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="ebc6a-163">O formato é definido em [Usando dicas de ordem no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ebc6a-163">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ebc6a-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="ebc6a-164">percentComplete</span></span>|<span data-ttu-id="ebc6a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ebc6a-165">Int32</span></span>|<span data-ttu-id="ebc6a-p111">A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="ebc6a-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ebc6a-168">startDateTime</span></span>|<span data-ttu-id="ebc6a-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc6a-169">DateTimeOffset</span></span>|<span data-ttu-id="ebc6a-170">A data e a hora que a tarefa começa.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-170">Date and time at which the task starts.</span></span> <span data-ttu-id="ebc6a-171">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ebc6a-172">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ebc6a-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ebc6a-173">title</span><span class="sxs-lookup"><span data-stu-id="ebc6a-173">title</span></span>|<span data-ttu-id="ebc6a-174">String</span><span class="sxs-lookup"><span data-stu-id="ebc6a-174">String</span></span>|<span data-ttu-id="ebc6a-175">Título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="ebc6a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc6a-176">Response</span></span>

<span data-ttu-id="ebc6a-177">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-177">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="ebc6a-178">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e o objeto `Prefer` `return=representation` `200 OK` [plannerTask](../resources/plannertask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-178">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="ebc6a-p114">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ebc6a-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ebc6a-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebc6a-182">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebc6a-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc6a-183">Request</span></span>
<span data-ttu-id="ebc6a-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-184">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebc6a-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc6a-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}
Content-type: application/json
Content-length: 247
Prefer: return=representation
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
# <a name="javascript"></a>[<span data-ttu-id="ebc6a-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebc6a-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ebc6a-187">C#</span><span class="sxs-lookup"><span data-stu-id="ebc6a-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebc6a-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc6a-188">Response</span></span>
<span data-ttu-id="ebc6a-189">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-189">Here is an example of the response.</span></span> <span data-ttu-id="ebc6a-190">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ebc6a-190">Note: The response object shown here might be shortened for readability.</span></span>
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

