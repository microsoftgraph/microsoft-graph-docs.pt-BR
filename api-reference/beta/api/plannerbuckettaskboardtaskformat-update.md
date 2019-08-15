---
title: Atualizar plannerBucketTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f0ee71fbcce4dd1c4771f766288d36a2d20fb3ad
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413388"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="8362e-103">Atualizar plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8362e-103">Update plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8362e-104">Atualize as propriedades do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="8362e-104">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8362e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8362e-105">Permissions</span></span>
<span data-ttu-id="8362e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8362e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8362e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8362e-108">Permission type</span></span>      | <span data-ttu-id="8362e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8362e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8362e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8362e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8362e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8362e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8362e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8362e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8362e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8362e-113">Not supported.</span></span>    |
|<span data-ttu-id="8362e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8362e-114">Application</span></span> | <span data-ttu-id="8362e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8362e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8362e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8362e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="8362e-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8362e-117">Optional request headers</span></span>
| <span data-ttu-id="8362e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8362e-118">Name</span></span>       | <span data-ttu-id="8362e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8362e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8362e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8362e-120">Authorization</span></span>  | <span data-ttu-id="8362e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8362e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8362e-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="8362e-123">If-Match</span></span>  | <span data-ttu-id="8362e-124">Último valor de ETag conhecido para o **plannerBucketTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="8362e-124">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="8362e-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8362e-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8362e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8362e-126">Request body</span></span>
<span data-ttu-id="8362e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8362e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8362e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8362e-130">Property</span></span>     | <span data-ttu-id="8362e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8362e-131">Type</span></span>   |<span data-ttu-id="8362e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8362e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8362e-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="8362e-133">orderHint</span></span>|<span data-ttu-id="8362e-134">String</span><span class="sxs-lookup"><span data-stu-id="8362e-134">String</span></span>|<span data-ttu-id="8362e-135">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="8362e-135">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="8362e-136">O formato é definido conforme descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="8362e-136">The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8362e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8362e-137">Response</span></span>

<span data-ttu-id="8362e-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8362e-138">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="8362e-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8362e-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8362e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8362e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8362e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8362e-143">Request</span></span>
<span data-ttu-id="8362e-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8362e-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8362e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="8362e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8362e-146">C#</span><span class="sxs-lookup"><span data-stu-id="8362e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8362e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8362e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8362e-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8362e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8362e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8362e-149">Response</span></span>
<span data-ttu-id="8362e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8362e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
