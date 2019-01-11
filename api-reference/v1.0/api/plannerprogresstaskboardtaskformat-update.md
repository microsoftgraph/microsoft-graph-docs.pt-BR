---
title: Atualizar plannerProgressTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
ms.openlocfilehash: 2964fe7f6002075bf3a18fa39be149e34fe55031
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815257"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="e00a2-103">Atualizar plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e00a2-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="e00a2-104">Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="e00a2-104">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e00a2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e00a2-105">Permissions</span></span>
<span data-ttu-id="e00a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e00a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e00a2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e00a2-108">Permission type</span></span>      | <span data-ttu-id="e00a2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e00a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e00a2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e00a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e00a2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e00a2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e00a2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e00a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e00a2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e00a2-113">Not supported.</span></span>    |
|<span data-ttu-id="e00a2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e00a2-114">Application</span></span> | <span data-ttu-id="e00a2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e00a2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e00a2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e00a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="e00a2-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e00a2-117">Optional request headers</span></span>
| <span data-ttu-id="e00a2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e00a2-118">Name</span></span>       | <span data-ttu-id="e00a2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e00a2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e00a2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e00a2-120">Authorization</span></span>  | <span data-ttu-id="e00a2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e00a2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e00a2-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="e00a2-123">If-Match</span></span>  | <span data-ttu-id="e00a2-p103">Último valor ETag conhecido do objeto **plannerProgressTaskBoardTaskFormat** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e00a2-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e00a2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e00a2-126">Request body</span></span>
<span data-ttu-id="e00a2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e00a2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e00a2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e00a2-130">Property</span></span>     | <span data-ttu-id="e00a2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e00a2-131">Type</span></span>   |<span data-ttu-id="e00a2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e00a2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e00a2-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="e00a2-133">orderHint</span></span>|<span data-ttu-id="e00a2-134">String</span><span class="sxs-lookup"><span data-stu-id="e00a2-134">String</span></span>|<span data-ttu-id="e00a2-p105">Valor da dica usado para ordenar a tarefa no modo de exibição Progress do Quadro de Tarefas. O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e00a2-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e00a2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e00a2-137">Response</span></span>

<span data-ttu-id="e00a2-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e00a2-138">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e00a2-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e00a2-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e00a2-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e00a2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e00a2-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e00a2-143">Request</span></span>
<span data-ttu-id="e00a2-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e00a2-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="e00a2-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e00a2-145">Response</span></span>
<span data-ttu-id="e00a2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e00a2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
