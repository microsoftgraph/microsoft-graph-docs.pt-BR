---
title: Atualizar plannerbucket
description: Atualize as propriedades do **objeto plannerbucket.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: bdf31387689e8bf0c7b43fd48cb406a2ce631146
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474064"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="e7de6-103">Atualizar plannerbucket</span><span class="sxs-lookup"><span data-stu-id="e7de6-103">Update plannerbucket</span></span>

<span data-ttu-id="e7de6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7de6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7de6-105">Atualize as propriedades do **objeto plannerbucket.**</span><span class="sxs-lookup"><span data-stu-id="e7de6-105">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7de6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7de6-106">Permissions</span></span>
<span data-ttu-id="e7de6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7de6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7de6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7de6-109">Permission type</span></span>      | <span data-ttu-id="e7de6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7de6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7de6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7de6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7de6-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7de6-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7de6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7de6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7de6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7de6-114">Not supported.</span></span>    |
|<span data-ttu-id="e7de6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7de6-115">Application</span></span> | <span data-ttu-id="e7de6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7de6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7de6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7de6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e7de6-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e7de6-118">Optional request headers</span></span>
| <span data-ttu-id="e7de6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e7de6-119">Name</span></span>       | <span data-ttu-id="e7de6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7de6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e7de6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7de6-121">Authorization</span></span>  | <span data-ttu-id="e7de6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7de6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7de6-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="e7de6-124">If-Match</span></span>  | <span data-ttu-id="e7de6-125">Último valor conhecido de ETag para o **plannerBucket** ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="e7de6-125">Last known ETag value for the **plannerBucket** to be updated.</span></span> <span data-ttu-id="e7de6-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7de6-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7de6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7de6-127">Request body</span></span>
<span data-ttu-id="e7de6-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e7de6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e7de6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7de6-131">Property</span></span>     | <span data-ttu-id="e7de6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7de6-132">Type</span></span>   |<span data-ttu-id="e7de6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7de6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7de6-134">nome</span><span class="sxs-lookup"><span data-stu-id="e7de6-134">name</span></span>|<span data-ttu-id="e7de6-135">String</span><span class="sxs-lookup"><span data-stu-id="e7de6-135">String</span></span>|<span data-ttu-id="e7de6-136">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="e7de6-136">Name of the bucket.</span></span>|
|<span data-ttu-id="e7de6-137">orderHint</span><span class="sxs-lookup"><span data-stu-id="e7de6-137">orderHint</span></span>|<span data-ttu-id="e7de6-138">String</span><span class="sxs-lookup"><span data-stu-id="e7de6-138">String</span></span>|<span data-ttu-id="e7de6-p105">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e7de6-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e7de6-141">planId</span><span class="sxs-lookup"><span data-stu-id="e7de6-141">planId</span></span>|<span data-ttu-id="e7de6-142">String</span><span class="sxs-lookup"><span data-stu-id="e7de6-142">String</span></span>|<span data-ttu-id="e7de6-143">Plan id to which the bucket belongs.</span><span class="sxs-lookup"><span data-stu-id="e7de6-143">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="e7de6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7de6-144">Response</span></span>

<span data-ttu-id="e7de6-145">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="e7de6-145">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="e7de6-146">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e o objeto `Prefer` `return=representation` `200 OK` [plannerBucket](../resources/plannerbucket.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7de6-146">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="e7de6-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e7de6-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e7de6-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7de6-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7de6-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7de6-151">Request</span></span>
<span data-ttu-id="e7de6-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7de6-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7de6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7de6-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
Content-type: application/json
Content-length: 27
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
# <a name="c"></a>[<span data-ttu-id="e7de6-154">C#</span><span class="sxs-lookup"><span data-stu-id="e7de6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7de6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7de6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7de6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7de6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7de6-157">Java</span><span class="sxs-lookup"><span data-stu-id="e7de6-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7de6-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7de6-158">Response</span></span>
<span data-ttu-id="e7de6-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7de6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

