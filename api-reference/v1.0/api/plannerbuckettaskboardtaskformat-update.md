---
title: Atualizar plannerBucketTaskBoardTaskFormat
description: Atualize as propriedades do **objeto plannerBucketTaskBoardTaskFormat.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f204de1d662b898b69d8ae0b5d5ba344c5e13212
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055845"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="6eb4b-103">Atualizar plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6eb4b-103">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="6eb4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eb4b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6eb4b-105">Atualize as propriedades do **objeto plannerBucketTaskBoardTaskFormat.**</span><span class="sxs-lookup"><span data-stu-id="6eb4b-105">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6eb4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6eb4b-106">Permissions</span></span>
<span data-ttu-id="6eb4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eb4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6eb4b-109">Permission type</span></span>      | <span data-ttu-id="6eb4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6eb4b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6eb4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6eb4b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6eb4b-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eb4b-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6eb4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6eb4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eb4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-114">Not supported.</span></span>    |
|<span data-ttu-id="6eb4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6eb4b-115">Application</span></span> | <span data-ttu-id="6eb4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6eb4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6eb4b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="6eb4b-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6eb4b-118">Optional request headers</span></span>
| <span data-ttu-id="6eb4b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6eb4b-119">Name</span></span>       | <span data-ttu-id="6eb4b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6eb4b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6eb4b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6eb4b-121">Authorization</span></span>  | <span data-ttu-id="6eb4b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6eb4b-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="6eb4b-124">If-Match</span></span>  | <span data-ttu-id="6eb4b-125">Último valor conhecido de ETag para que **o plannerBucketTaskBoardTaskFormat** seja atualizado.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-125">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="6eb4b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eb4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb4b-127">Request body</span></span>
<span data-ttu-id="6eb4b-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6eb4b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6eb4b-131">Property</span></span>     | <span data-ttu-id="6eb4b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6eb4b-132">Type</span></span>   |<span data-ttu-id="6eb4b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6eb4b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6eb4b-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="6eb4b-134">orderHint</span></span>|<span data-ttu-id="6eb4b-135">String</span><span class="sxs-lookup"><span data-stu-id="6eb4b-135">String</span></span>|<span data-ttu-id="6eb4b-136">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-136">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="6eb4b-137">O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="6eb4b-137">The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="6eb4b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eb4b-138">Response</span></span>

<span data-ttu-id="6eb4b-139">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-139">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="6eb4b-140">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e o objeto `Prefer` `return=representation` `200 OK` [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-140">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="6eb4b-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6eb4b-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6eb4b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6eb4b-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6eb4b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb4b-145">Request</span></span>
<span data-ttu-id="6eb4b-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6eb4b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6eb4b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="6eb4b-148">C#</span><span class="sxs-lookup"><span data-stu-id="6eb4b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6eb4b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6eb4b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6eb4b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6eb4b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6eb4b-151">Java</span><span class="sxs-lookup"><span data-stu-id="6eb4b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6eb4b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eb4b-152">Response</span></span>
<span data-ttu-id="6eb4b-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-153">Here is an example of the response.</span></span> <span data-ttu-id="6eb4b-154">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6eb4b-154">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

