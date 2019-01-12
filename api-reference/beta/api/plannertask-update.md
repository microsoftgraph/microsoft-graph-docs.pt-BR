---
title: Atualizar plannertask
description: Atualize as propriedades do objeto **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1592657fd8ae71cff17fe79631a38eb2ce6e6197
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931577"
---
# <a name="update-plannertask"></a><span data-ttu-id="c7754-103">Atualizar plannertask</span><span class="sxs-lookup"><span data-stu-id="c7754-103">Update plannertask</span></span>

> <span data-ttu-id="c7754-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7754-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7754-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7754-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7754-106">Atualize as propriedades do objeto **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="c7754-106">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7754-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7754-107">Permissions</span></span>
<span data-ttu-id="c7754-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7754-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7754-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7754-110">Permission type</span></span>      | <span data-ttu-id="c7754-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7754-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7754-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7754-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7754-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7754-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7754-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7754-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7754-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7754-115">Not supported.</span></span>    |
|<span data-ttu-id="c7754-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7754-116">Application</span></span> | <span data-ttu-id="c7754-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7754-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7754-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7754-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="c7754-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c7754-119">Optional request headers</span></span>
| <span data-ttu-id="c7754-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c7754-120">Name</span></span>       | <span data-ttu-id="c7754-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7754-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c7754-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7754-122">Authorization</span></span>  | <span data-ttu-id="c7754-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7754-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7754-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="c7754-125">If-Match</span></span>  | <span data-ttu-id="c7754-p104">O último valor ETag conhecido do objeto **plannerTask** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7754-p104">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7754-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7754-128">Request body</span></span>
<span data-ttu-id="c7754-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c7754-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c7754-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7754-132">Property</span></span>     | <span data-ttu-id="c7754-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7754-133">Type</span></span>   |<span data-ttu-id="c7754-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7754-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7754-135">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="c7754-135">appliedCategories</span></span>|[<span data-ttu-id="c7754-136">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="c7754-136">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="c7754-p106">As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="c7754-p106">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="c7754-139">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="c7754-139">assigneePriority</span></span>|<span data-ttu-id="c7754-140">String</span><span class="sxs-lookup"><span data-stu-id="c7754-140">String</span></span>|<span data-ttu-id="c7754-p107">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c7754-p107">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c7754-143">assignments</span><span class="sxs-lookup"><span data-stu-id="c7754-143">assignments</span></span>|[<span data-ttu-id="c7754-144">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="c7754-144">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="c7754-145">O conjunto de usuários ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="c7754-145">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="c7754-146">bucketId</span><span class="sxs-lookup"><span data-stu-id="c7754-146">bucketId</span></span>|<span data-ttu-id="c7754-147">String</span><span class="sxs-lookup"><span data-stu-id="c7754-147">String</span></span>|<span data-ttu-id="c7754-148">Id de Balde ao qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="c7754-148">Bucket id to which the task belongs.</span></span> <span data-ttu-id="c7754-149">O Balde deve estar no plano de que a tarefa está em.</span><span class="sxs-lookup"><span data-stu-id="c7754-149">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="c7754-150">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c7754-150">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c7754-151">[Validação de formato](../resources/tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="c7754-151">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="c7754-152">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="c7754-152">conversationThreadId</span></span>|<span data-ttu-id="c7754-153">String</span><span class="sxs-lookup"><span data-stu-id="c7754-153">String</span></span>|<span data-ttu-id="c7754-p109">Identificação do thread da conversa na tarefa. Essa é a identificação do objeto do thread da conversa criado no grupo.</span><span class="sxs-lookup"><span data-stu-id="c7754-p109">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="c7754-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="c7754-156">dueDateTime</span></span>|<span data-ttu-id="c7754-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7754-157">DateTimeOffset</span></span>|<span data-ttu-id="c7754-p110">A data e a hora que a tarefa já deve estar concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c7754-p110">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c7754-161">orderHint</span><span class="sxs-lookup"><span data-stu-id="c7754-161">orderHint</span></span>|<span data-ttu-id="c7754-162">String</span><span class="sxs-lookup"><span data-stu-id="c7754-162">String</span></span>|<span data-ttu-id="c7754-p111">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c7754-p111">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c7754-165">percentComplete</span><span class="sxs-lookup"><span data-stu-id="c7754-165">percentComplete</span></span>|<span data-ttu-id="c7754-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c7754-166">Int32</span></span>|<span data-ttu-id="c7754-p112">A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída.</span><span class="sxs-lookup"><span data-stu-id="c7754-p112">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="c7754-169">planId</span><span class="sxs-lookup"><span data-stu-id="c7754-169">planId</span></span>|<span data-ttu-id="c7754-170">String</span><span class="sxs-lookup"><span data-stu-id="c7754-170">String</span></span>|<span data-ttu-id="c7754-171">ID do plano ao qual a tarefa pertence.</span><span class="sxs-lookup"><span data-stu-id="c7754-171">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="c7754-172">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7754-172">startDateTime</span></span>|<span data-ttu-id="c7754-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7754-173">DateTimeOffset</span></span>|<span data-ttu-id="c7754-p113">A data e a hora que a tarefa começa. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c7754-p113">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c7754-177">title</span><span class="sxs-lookup"><span data-stu-id="c7754-177">title</span></span>|<span data-ttu-id="c7754-178">String</span><span class="sxs-lookup"><span data-stu-id="c7754-178">String</span></span>|<span data-ttu-id="c7754-179">Título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="c7754-179">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="c7754-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7754-180">Response</span></span>

<span data-ttu-id="c7754-181">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerTask](../resources/plannertask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7754-181">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="c7754-p114">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c7754-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c7754-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7754-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7754-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7754-186">Request</span></span>
<span data-ttu-id="c7754-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7754-187">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c7754-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7754-188">Response</span></span>
<span data-ttu-id="c7754-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7754-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
