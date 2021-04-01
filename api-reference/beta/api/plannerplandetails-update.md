---
title: Atualizar plannerplandetails
description: Atualize as propriedades do **objeto plannerplandetails.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: ee12fd4607f4f3b2fad4f32e0473698fbe95b601
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473581"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="34ab2-103">Atualizar plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="34ab2-103">Update plannerplandetails</span></span>

<span data-ttu-id="34ab2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34ab2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34ab2-105">Atualize as propriedades do **objeto plannerplandetails.**</span><span class="sxs-lookup"><span data-stu-id="34ab2-105">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34ab2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34ab2-106">Permissions</span></span>
<span data-ttu-id="34ab2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ab2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34ab2-109">Permission type</span></span>      | <span data-ttu-id="34ab2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34ab2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ab2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34ab2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34ab2-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ab2-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34ab2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34ab2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ab2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ab2-114">Not supported.</span></span>    |
|<span data-ttu-id="34ab2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34ab2-115">Application</span></span> | <span data-ttu-id="34ab2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ab2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34ab2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34ab2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="34ab2-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="34ab2-118">Optional request headers</span></span>
| <span data-ttu-id="34ab2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="34ab2-119">Name</span></span>       | <span data-ttu-id="34ab2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="34ab2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="34ab2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34ab2-121">Authorization</span></span>  | <span data-ttu-id="34ab2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34ab2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34ab2-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="34ab2-124">If-Match</span></span>  | <span data-ttu-id="34ab2-125">Último valor ETag conhecido para o plannerPlanDetails a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="34ab2-125">Last known ETag value for the plannerPlanDetails to be updated.</span></span> <span data-ttu-id="34ab2-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34ab2-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ab2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34ab2-127">Request body</span></span>
<span data-ttu-id="34ab2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="34ab2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="34ab2-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34ab2-131">Property</span></span>     | <span data-ttu-id="34ab2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="34ab2-132">Type</span></span>   |<span data-ttu-id="34ab2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="34ab2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34ab2-134">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="34ab2-134">categoryDescriptions</span></span>|[<span data-ttu-id="34ab2-135">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="34ab2-135">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="34ab2-136">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="34ab2-136">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="34ab2-137">sharedWith</span><span class="sxs-lookup"><span data-stu-id="34ab2-137">sharedWith</span></span>|[<span data-ttu-id="34ab2-138">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="34ab2-138">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="34ab2-139">Conjunto de ids de usuário com as que esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="34ab2-139">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="34ab2-140">Se você estiver aproveitando grupos do Microsoft 365, use a API grupos para gerenciar a associação ao grupo para compartilhar o [plano do](../resources/group.md) grupo.</span><span class="sxs-lookup"><span data-stu-id="34ab2-140">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan.</span></span> <span data-ttu-id="34ab2-141">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="34ab2-141">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="34ab2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ab2-142">Response</span></span>

<span data-ttu-id="34ab2-143">Se tiver êxito, este método retornará `204 No Content` resposta e conteúdo vazio.</span><span class="sxs-lookup"><span data-stu-id="34ab2-143">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="34ab2-144">Se a solicitação especificar o header com preferência, este método retornará um código de resposta e o objeto `Prefer` `return=representation` `200 OK` [plannerPlanDetails](../resources/plannerplandetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34ab2-144">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="34ab2-p107">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="34ab2-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="34ab2-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34ab2-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34ab2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34ab2-149">Request</span></span>
<span data-ttu-id="34ab2-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34ab2-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34ab2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="34ab2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
Content-type: application/json
Content-length: 212
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
# <a name="c"></a>[<span data-ttu-id="34ab2-152">C#</span><span class="sxs-lookup"><span data-stu-id="34ab2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34ab2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34ab2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34ab2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34ab2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34ab2-155">Java</span><span class="sxs-lookup"><span data-stu-id="34ab2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="34ab2-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ab2-156">Response</span></span>
<span data-ttu-id="34ab2-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34ab2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


