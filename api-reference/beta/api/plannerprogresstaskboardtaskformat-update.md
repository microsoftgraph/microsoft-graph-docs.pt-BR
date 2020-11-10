---
title: Atualizar plannerProgressTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 4d0f874a4de109ea60d2b0f1af47f654791ca3d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973451"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="5c7cb-103">Atualizar plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5c7cb-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="5c7cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c7cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c7cb-105">Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5c7cb-105">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c7cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c7cb-106">Permissions</span></span>
<span data-ttu-id="5c7cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c7cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c7cb-109">Permission type</span></span>      | <span data-ttu-id="5c7cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c7cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c7cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c7cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c7cb-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c7cb-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c7cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c7cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c7cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-114">Not supported.</span></span>    |
|<span data-ttu-id="5c7cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c7cb-115">Application</span></span> | <span data-ttu-id="5c7cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c7cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c7cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="5c7cb-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5c7cb-118">Optional request headers</span></span>
| <span data-ttu-id="5c7cb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c7cb-119">Name</span></span>       | <span data-ttu-id="5c7cb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c7cb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5c7cb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c7cb-121">Authorization</span></span>  | <span data-ttu-id="5c7cb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c7cb-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="5c7cb-124">If-Match</span></span>  | <span data-ttu-id="5c7cb-125">Último valor de ETag conhecido para o **plannerProgressTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-125">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="5c7cb-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c7cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7cb-127">Request body</span></span>
<span data-ttu-id="5c7cb-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5c7cb-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c7cb-131">Property</span></span>     | <span data-ttu-id="5c7cb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c7cb-132">Type</span></span>   |<span data-ttu-id="5c7cb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c7cb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c7cb-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="5c7cb-134">orderHint</span></span>|<span data-ttu-id="5c7cb-135">String</span><span class="sxs-lookup"><span data-stu-id="5c7cb-135">String</span></span>|<span data-ttu-id="5c7cb-136">O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-136">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="5c7cb-137">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5c7cb-137">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="5c7cb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c7cb-138">Response</span></span>

<span data-ttu-id="5c7cb-139">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-139">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="5c7cb-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="5c7cb-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5c7cb-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c7cb-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c7cb-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c7cb-144">Request</span></span>
<span data-ttu-id="5c7cb-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c7cb-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c7cb-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/{id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="5c7cb-147">C#</span><span class="sxs-lookup"><span data-stu-id="5c7cb-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c7cb-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c7cb-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c7cb-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c7cb-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c7cb-150">Java</span><span class="sxs-lookup"><span data-stu-id="5c7cb-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c7cb-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c7cb-151">Response</span></span>
<span data-ttu-id="5c7cb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c7cb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


