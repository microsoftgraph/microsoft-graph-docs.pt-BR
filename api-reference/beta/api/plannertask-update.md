---
title: Atualizar plannertask
description: Atualize as propriedades do objeto **plannertask** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 955412f1f699f374b974cfdde81c8baedc4021dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095811"
---
# <a name="update-plannertask"></a><span data-ttu-id="4cb0b-103">Atualizar plannertask</span><span class="sxs-lookup"><span data-stu-id="4cb0b-103">Update plannertask</span></span>

<span data-ttu-id="4cb0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cb0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb0b-105">Atualize as propriedades do objeto **plannertask** .</span><span class="sxs-lookup"><span data-stu-id="4cb0b-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cb0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cb0b-106">Permissions</span></span>
<span data-ttu-id="4cb0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cb0b-109">Permission type</span></span>      | <span data-ttu-id="4cb0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cb0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cb0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cb0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4cb0b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb0b-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cb0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cb0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-114">Not supported.</span></span>    |
|<span data-ttu-id="4cb0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cb0b-115">Application</span></span> | <span data-ttu-id="4cb0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cb0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cb0b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4cb0b-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4cb0b-118">Optional request headers</span></span>
| <span data-ttu-id="4cb0b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4cb0b-119">Name</span></span>       | <span data-ttu-id="4cb0b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cb0b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4cb0b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cb0b-121">Authorization</span></span>  | <span data-ttu-id="4cb0b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cb0b-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="4cb0b-124">If-Match</span></span>  | <span data-ttu-id="4cb0b-125">Último valor de ETag conhecido para o **plannerTask** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-125">Last known ETag value for the **plannerTask** to be updated.</span></span> <span data-ttu-id="4cb0b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cb0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cb0b-127">Request body</span></span>
<span data-ttu-id="4cb0b-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4cb0b-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4cb0b-130">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-130">For best performance,  don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4cb0b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cb0b-131">Property</span></span>     | <span data-ttu-id="4cb0b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cb0b-132">Type</span></span>   |<span data-ttu-id="4cb0b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cb0b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cb0b-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="4cb0b-134">appliedCategories</span></span>|[<span data-ttu-id="4cb0b-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="4cb0b-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="4cb0b-p105">As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="4cb0b-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="4cb0b-138">assigneePriority</span></span>|<span data-ttu-id="4cb0b-139">String</span><span class="sxs-lookup"><span data-stu-id="4cb0b-139">String</span></span>|<span data-ttu-id="4cb0b-p106">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p106">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="4cb0b-142">assignments</span><span class="sxs-lookup"><span data-stu-id="4cb0b-142">assignments</span></span>|[<span data-ttu-id="4cb0b-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="4cb0b-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="4cb0b-144">O conjunto de usuários ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="4cb0b-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="4cb0b-145">bucketId</span></span>|<span data-ttu-id="4cb0b-146">String</span><span class="sxs-lookup"><span data-stu-id="4cb0b-146">String</span></span>|<span data-ttu-id="4cb0b-147">ID de Bucket à qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="4cb0b-148">O bucket precisa estar no plano no qual a tarefa está.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="4cb0b-149">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="4cb0b-150">[Formatar validação](../resources/tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-150">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="4cb0b-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="4cb0b-151">conversationThreadId</span></span>|<span data-ttu-id="4cb0b-152">String</span><span class="sxs-lookup"><span data-stu-id="4cb0b-152">String</span></span>|<span data-ttu-id="4cb0b-153">ID do thread da conversa na tarefa.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-153">Thread id of the conversation on the task.</span></span> <span data-ttu-id="4cb0b-154">Esta é a ID do objeto de thread de conversa criado no grupo.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-154">This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="4cb0b-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb0b-155">dueDateTime</span></span>|<span data-ttu-id="4cb0b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb0b-156">DateTimeOffset</span></span>|<span data-ttu-id="4cb0b-p109">A data e a hora que a tarefa já deve estar concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4cb0b-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="4cb0b-160">orderHint</span></span>|<span data-ttu-id="4cb0b-161">String</span><span class="sxs-lookup"><span data-stu-id="4cb0b-161">String</span></span>|<span data-ttu-id="4cb0b-p110">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p110">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="4cb0b-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="4cb0b-164">percentComplete</span></span>|<span data-ttu-id="4cb0b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb0b-165">Int32</span></span>|<span data-ttu-id="4cb0b-p111">A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="4cb0b-168">prioridade</span><span class="sxs-lookup"><span data-stu-id="4cb0b-168">priority</span></span>|<span data-ttu-id="4cb0b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb0b-169">Int32</span></span>|<span data-ttu-id="4cb0b-170">Prioridade da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-170">Priority of the task.</span></span> <span data-ttu-id="4cb0b-171">O intervalo de valores válido é entre `0` e `10` (inclusive), com o valor crescente sendo prioridade mais baixa ( `0` tem a maior prioridade e `10` tem a menor prioridade).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-171">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="4cb0b-172">Atualmente, o Planner interpreta valores `0` e `1` como "urgente" `2` e como "importante", e como "médio" e `3` `4` `5` `6` `7` `8` , `9` e `10` como "baixo".</span><span class="sxs-lookup"><span data-stu-id="4cb0b-172">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="4cb0b-173">Atualmente, o Planner define o valor `1` para "urgente", `3` para "importante", `5` para "médio" e `9` para "baixo".</span><span class="sxs-lookup"><span data-stu-id="4cb0b-173">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="4cb0b-174">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb0b-174">startDateTime</span></span>|<span data-ttu-id="4cb0b-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb0b-175">DateTimeOffset</span></span>|<span data-ttu-id="4cb0b-p113">A data e a hora que a tarefa começa. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p113">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4cb0b-179">title</span><span class="sxs-lookup"><span data-stu-id="4cb0b-179">title</span></span>|<span data-ttu-id="4cb0b-180">String</span><span class="sxs-lookup"><span data-stu-id="4cb0b-180">String</span></span>|<span data-ttu-id="4cb0b-181">Título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-181">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="4cb0b-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cb0b-182">Response</span></span>

<span data-ttu-id="4cb0b-183">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [plannerTask](../resources/plannertask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-183">If successful, this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="4cb0b-p114">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4cb0b-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cb0b-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cb0b-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cb0b-188">Request</span></span>
<span data-ttu-id="4cb0b-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-189">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cb0b-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cb0b-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
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
# <a name="javascript"></a>[<span data-ttu-id="4cb0b-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cb0b-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4cb0b-192">C#</span><span class="sxs-lookup"><span data-stu-id="4cb0b-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4cb0b-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cb0b-193">Response</span></span>
<span data-ttu-id="4cb0b-194">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-194">Here is an example of the response.</span></span> 

><span data-ttu-id="4cb0b-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cb0b-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


