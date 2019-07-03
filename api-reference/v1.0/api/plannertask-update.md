---
title: Atualizar plannertask
description: Atualize as propriedades do objeto **plannertask** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: c9a8c9b7a9c3e0e0a7f212b64491ba97e949c74f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454332"
---
# <a name="update-plannertask"></a><span data-ttu-id="bfdb9-103">Atualizar plannertask</span><span class="sxs-lookup"><span data-stu-id="bfdb9-103">Update plannertask</span></span>

<span data-ttu-id="bfdb9-104">Atualize as propriedades do objeto **plannertask** .</span><span class="sxs-lookup"><span data-stu-id="bfdb9-104">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfdb9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfdb9-105">Permissions</span></span>
<span data-ttu-id="bfdb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfdb9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfdb9-108">Permission type</span></span>      | <span data-ttu-id="bfdb9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfdb9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfdb9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdb9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfdb9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfdb9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-113">Not supported.</span></span>    |
|<span data-ttu-id="bfdb9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfdb9-114">Application</span></span> | <span data-ttu-id="bfdb9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfdb9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfdb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="bfdb9-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bfdb9-117">Optional request headers</span></span>
| <span data-ttu-id="bfdb9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bfdb9-118">Name</span></span>       | <span data-ttu-id="bfdb9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfdb9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bfdb9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfdb9-120">Authorization</span></span>  | <span data-ttu-id="bfdb9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfdb9-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="bfdb9-123">If-Match</span></span>  | <span data-ttu-id="bfdb9-124">Último valor de ETag conhecido para o **plannerTask** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-124">Last known ETag value for the **plannerTask** to be updated.</span></span> <span data-ttu-id="bfdb9-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfdb9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfdb9-126">Request body</span></span>
<span data-ttu-id="bfdb9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bfdb9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfdb9-130">Property</span></span>     | <span data-ttu-id="bfdb9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfdb9-131">Type</span></span>   |<span data-ttu-id="bfdb9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfdb9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfdb9-133">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="bfdb9-133">appliedCategories</span></span>|[<span data-ttu-id="bfdb9-134">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="bfdb9-134">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="bfdb9-p105">As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="bfdb9-137">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="bfdb9-137">assigneePriority</span></span>|<span data-ttu-id="bfdb9-138">String</span><span class="sxs-lookup"><span data-stu-id="bfdb9-138">String</span></span>|<span data-ttu-id="bfdb9-139">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-139">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="bfdb9-140">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="bfdb9-140">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="bfdb9-141">assignments</span><span class="sxs-lookup"><span data-stu-id="bfdb9-141">assignments</span></span>|[<span data-ttu-id="bfdb9-142">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="bfdb9-142">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="bfdb9-143">O conjunto de usuários ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-143">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="bfdb9-144">bucketId</span><span class="sxs-lookup"><span data-stu-id="bfdb9-144">bucketId</span></span>|<span data-ttu-id="bfdb9-145">String</span><span class="sxs-lookup"><span data-stu-id="bfdb9-145">String</span></span>|<span data-ttu-id="bfdb9-146">ID de Bucket à qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-146">Bucket id to which the task belongs.</span></span> <span data-ttu-id="bfdb9-147">O bucket precisa estar no plano no qual a tarefa está.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-147">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="bfdb9-148">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-148">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="bfdb9-149">[Formatar validação](../resources/planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-149">[Format validation](../resources/planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="bfdb9-150">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="bfdb9-150">conversationThreadId</span></span>|<span data-ttu-id="bfdb9-151">String</span><span class="sxs-lookup"><span data-stu-id="bfdb9-151">String</span></span>|<span data-ttu-id="bfdb9-152">ID do thread da conversa na tarefa.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-152">Thread id of the conversation on the task.</span></span> <span data-ttu-id="bfdb9-153">Esta é a ID do objeto de thread de conversa criado no grupo.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-153">This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="bfdb9-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdb9-154">dueDateTime</span></span>|<span data-ttu-id="bfdb9-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdb9-155">DateTimeOffset</span></span>|<span data-ttu-id="bfdb9-p109">A data e a hora que a tarefa já deve estar concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfdb9-159">orderHint</span><span class="sxs-lookup"><span data-stu-id="bfdb9-159">orderHint</span></span>|<span data-ttu-id="bfdb9-160">String</span><span class="sxs-lookup"><span data-stu-id="bfdb9-160">String</span></span>|<span data-ttu-id="bfdb9-161">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-161">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="bfdb9-162">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="bfdb9-162">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="bfdb9-163">percentComplete</span><span class="sxs-lookup"><span data-stu-id="bfdb9-163">percentComplete</span></span>|<span data-ttu-id="bfdb9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb9-164">Int32</span></span>|<span data-ttu-id="bfdb9-p111">A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="bfdb9-167">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdb9-167">startDateTime</span></span>|<span data-ttu-id="bfdb9-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdb9-168">DateTimeOffset</span></span>|<span data-ttu-id="bfdb9-p112">A data e a hora que a tarefa começa. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfdb9-172">title</span><span class="sxs-lookup"><span data-stu-id="bfdb9-172">title</span></span>|<span data-ttu-id="bfdb9-173">String</span><span class="sxs-lookup"><span data-stu-id="bfdb9-173">String</span></span>|<span data-ttu-id="bfdb9-174">Título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-174">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="bfdb9-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfdb9-175">Response</span></span>

<span data-ttu-id="bfdb9-176">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerTask](../resources/plannertask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-176">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="bfdb9-p113">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p113">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bfdb9-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfdb9-180">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfdb9-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfdb9-181">Request</span></span>
<span data-ttu-id="bfdb9-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-182">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bfdb9-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfdb9-183">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfdb9-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="bfdb9-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bfdb9-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfdb9-185">Response</span></span>
<span data-ttu-id="bfdb9-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
