# <a name="update-plannertask"></a><span data-ttu-id="9d4a8-101">Atualizar plannertask</span><span class="sxs-lookup"><span data-stu-id="9d4a8-101">Update plannertask</span></span>

<span data-ttu-id="9d4a8-102">Atualize as propriedades do objeto **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-102">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d4a8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d4a8-103">Permissions</span></span>
<span data-ttu-id="9d4a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d4a8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d4a8-106">Permission type</span></span>      | <span data-ttu-id="9d4a8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d4a8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d4a8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d4a8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d4a8-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d4a8-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d4a8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d4a8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d4a8-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-111">Not supported.</span></span>    |
|<span data-ttu-id="9d4a8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d4a8-112">Application</span></span> | <span data-ttu-id="9d4a8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d4a8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d4a8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="9d4a8-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="9d4a8-115">Optional request headers</span></span>
| <span data-ttu-id="9d4a8-116">Nome</span><span class="sxs-lookup"><span data-stu-id="9d4a8-116">Name</span></span>       | <span data-ttu-id="9d4a8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d4a8-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d4a8-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d4a8-118">Authorization</span></span>  | <span data-ttu-id="9d4a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d4a8-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="9d4a8-121">If-Match</span></span>  | <span data-ttu-id="9d4a8-p103">O último valor ETag conhecido do objeto **plannerTask** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d4a8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d4a8-124">Request body</span></span>
<span data-ttu-id="9d4a8-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d4a8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d4a8-128">Property</span></span>     | <span data-ttu-id="9d4a8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d4a8-129">Type</span></span>   |<span data-ttu-id="9d4a8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d4a8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d4a8-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="9d4a8-131">appliedCategories</span></span>|[<span data-ttu-id="9d4a8-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="9d4a8-132">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="9d4a8-p105">As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="9d4a8-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="9d4a8-135">assigneePriority</span></span>|<span data-ttu-id="9d4a8-136">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d4a8-136">String</span></span>|<span data-ttu-id="9d4a8-p106">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido em [Como usar dicas de ordem no Planner](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="9d4a8-139">assignments</span><span class="sxs-lookup"><span data-stu-id="9d4a8-139">assignments</span></span>|[<span data-ttu-id="9d4a8-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="9d4a8-140">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="9d4a8-141">O conjunto de usuários ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-141">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="9d4a8-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="9d4a8-142">bucketId</span></span>|<span data-ttu-id="9d4a8-143">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d4a8-143">String</span></span>|<span data-ttu-id="9d4a8-144">Id do bucket ao qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-144">Bucket id to which the task belongs.</span></span> <span data-ttu-id="9d4a8-145">O bucket deve estar no plano em que está a tarefa.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-145">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="9d4a8-146">Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-146">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9d4a8-147">[Validação de formato](../resources/planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-147">[Format validation](../resources/planner_identifiers_disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="9d4a8-148">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="9d4a8-148">conversationThreadId</span></span>|<span data-ttu-id="9d4a8-149">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d4a8-149">String</span></span>|<span data-ttu-id="9d4a8-p108">Identificação do thread da conversa na tarefa. Essa é a identificação do objeto do thread da conversa criado no grupo.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="9d4a8-152">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="9d4a8-152">dueDateTime</span></span>|<span data-ttu-id="9d4a8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d4a8-153">DateTimeOffset</span></span>|<span data-ttu-id="9d4a8-p109">A data e a hora que a tarefa já deve estar concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9d4a8-157">orderHint</span><span class="sxs-lookup"><span data-stu-id="9d4a8-157">orderHint</span></span>|<span data-ttu-id="9d4a8-158">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d4a8-158">String</span></span>|<span data-ttu-id="9d4a8-p110">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido em [Como usar dicas de ordem no Planner](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p110">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="9d4a8-161">percentComplete</span><span class="sxs-lookup"><span data-stu-id="9d4a8-161">percentComplete</span></span>|<span data-ttu-id="9d4a8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9d4a8-162">Int32</span></span>|<span data-ttu-id="9d4a8-p111">A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="9d4a8-165">planId</span><span class="sxs-lookup"><span data-stu-id="9d4a8-165">planId</span></span>|<span data-ttu-id="9d4a8-166">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d4a8-166">String</span></span>|<span data-ttu-id="9d4a8-167">ID do plano ao qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-167">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="9d4a8-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d4a8-168">startDateTime</span></span>|<span data-ttu-id="9d4a8-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d4a8-169">DateTimeOffset</span></span>|<span data-ttu-id="9d4a8-p112">A data e a hora que a tarefa começa. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9d4a8-173">title</span><span class="sxs-lookup"><span data-stu-id="9d4a8-173">title</span></span>|<span data-ttu-id="9d4a8-174">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d4a8-174">String</span></span>|<span data-ttu-id="9d4a8-175">Título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="9d4a8-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d4a8-176">Response</span></span>

<span data-ttu-id="9d4a8-177">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerTask](../resources/plannertask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-177">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="9d4a8-p113">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p113">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9d4a8-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d4a8-181">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d4a8-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d4a8-182">Request</span></span>
<span data-ttu-id="9d4a8-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-183">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9d4a8-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d4a8-184">Response</span></span>
<span data-ttu-id="9d4a8-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d4a8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->