---
title: Atualizar plannerplandetails
description: Atualize as propriedades do objeto **plannerplandetails** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 54d63345a6848f1aa894b36c251234f59eac1720
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455645"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="02d7a-103">Atualizar plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="02d7a-103">Update plannerplandetails</span></span>

<span data-ttu-id="02d7a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02d7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02d7a-105">Atualize as propriedades do objeto **plannerplandetails** .</span><span class="sxs-lookup"><span data-stu-id="02d7a-105">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="02d7a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02d7a-106">Permissions</span></span>
<span data-ttu-id="02d7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02d7a-109">Permission type</span></span>      | <span data-ttu-id="02d7a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02d7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02d7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02d7a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02d7a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d7a-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02d7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02d7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02d7a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d7a-114">Not supported.</span></span>    |
|<span data-ttu-id="02d7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02d7a-115">Application</span></span> | <span data-ttu-id="02d7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d7a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02d7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02d7a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="02d7a-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="02d7a-118">Optional request headers</span></span>
| <span data-ttu-id="02d7a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="02d7a-119">Name</span></span>       | <span data-ttu-id="02d7a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d7a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02d7a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02d7a-121">Authorization</span></span>  | <span data-ttu-id="02d7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d7a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02d7a-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="02d7a-124">If-Match</span></span>  | <span data-ttu-id="02d7a-125">Último valor de ETag conhecido para o plannerPlanDetails a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="02d7a-125">Last known ETag value for the plannerPlanDetails to be updated.</span></span> <span data-ttu-id="02d7a-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d7a-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02d7a-127">Request body</span></span>
<span data-ttu-id="02d7a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="02d7a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="02d7a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02d7a-131">Property</span></span>     | <span data-ttu-id="02d7a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d7a-132">Type</span></span>   |<span data-ttu-id="02d7a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d7a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02d7a-134">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="02d7a-134">categoryDescriptions</span></span>|[<span data-ttu-id="02d7a-135">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="02d7a-135">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="02d7a-136">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="02d7a-136">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="02d7a-137">sharedWith</span><span class="sxs-lookup"><span data-stu-id="02d7a-137">sharedWith</span></span>|[<span data-ttu-id="02d7a-138">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="02d7a-138">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="02d7a-139">Conjunto de IDs de usuário com as quais esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="02d7a-139">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="02d7a-140">Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="02d7a-140">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan.</span></span> <span data-ttu-id="02d7a-141">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="02d7a-141">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="02d7a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d7a-142">Response</span></span>

<span data-ttu-id="02d7a-143">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerPlanDetails](../resources/plannerplandetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02d7a-143">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="02d7a-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="02d7a-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="02d7a-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02d7a-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02d7a-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02d7a-148">Request</span></span>
<span data-ttu-id="02d7a-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02d7a-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02d7a-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="02d7a-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
Content-type: application/json
Content-length: 212
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
# <a name="c"></a>[<span data-ttu-id="02d7a-151">C#</span><span class="sxs-lookup"><span data-stu-id="02d7a-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02d7a-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02d7a-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02d7a-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02d7a-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02d7a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d7a-154">Response</span></span>
<span data-ttu-id="02d7a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02d7a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
