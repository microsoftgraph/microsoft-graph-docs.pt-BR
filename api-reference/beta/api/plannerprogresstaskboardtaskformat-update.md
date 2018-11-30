---
title: Atualizar plannerProgressTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat**.
ms.openlocfilehash: 628b17075e02bfad5859f68c118f742a11691a53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033671"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="46d0e-103">Atualizar plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="46d0e-103">Update plannerProgressTaskBoardTaskFormat</span></span>

> <span data-ttu-id="46d0e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46d0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46d0e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46d0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46d0e-106">Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="46d0e-106">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="46d0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="46d0e-107">Permissions</span></span>
<span data-ttu-id="46d0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46d0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46d0e-110">Permission type</span></span>      | <span data-ttu-id="46d0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46d0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46d0e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46d0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46d0e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d0e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="46d0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46d0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46d0e-115">Not supported.</span></span>    |
|<span data-ttu-id="46d0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46d0e-116">Application</span></span> | <span data-ttu-id="46d0e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46d0e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46d0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46d0e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="46d0e-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="46d0e-119">Optional request headers</span></span>
| <span data-ttu-id="46d0e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="46d0e-120">Name</span></span>       | <span data-ttu-id="46d0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d0e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="46d0e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46d0e-122">Authorization</span></span>  | <span data-ttu-id="46d0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46d0e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46d0e-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="46d0e-125">If-Match</span></span>  | <span data-ttu-id="46d0e-p104">Último valor ETag conhecido do objeto **plannerProgressTaskBoardTaskFormat** a ser atualizado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46d0e-p104">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46d0e-128">Request body</span></span>
<span data-ttu-id="46d0e-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="46d0e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46d0e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46d0e-132">Property</span></span>     | <span data-ttu-id="46d0e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="46d0e-133">Type</span></span>   |<span data-ttu-id="46d0e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d0e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46d0e-135">orderHint</span><span class="sxs-lookup"><span data-stu-id="46d0e-135">orderHint</span></span>|<span data-ttu-id="46d0e-136">String</span><span class="sxs-lookup"><span data-stu-id="46d0e-136">String</span></span>|<span data-ttu-id="46d0e-137">Dica valor usado para solicitar a tarefa, o modo de exibição do progresso da tarefa placa.</span><span class="sxs-lookup"><span data-stu-id="46d0e-137">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="46d0e-138">O formato é definido em [dicas de ordem de uso no planejador](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="46d0e-138">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="46d0e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="46d0e-139">Response</span></span>

<span data-ttu-id="46d0e-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46d0e-140">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="46d0e-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="46d0e-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="46d0e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46d0e-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46d0e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46d0e-145">Request</span></span>
<span data-ttu-id="46d0e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46d0e-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="46d0e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="46d0e-147">Response</span></span>
<span data-ttu-id="46d0e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46d0e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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