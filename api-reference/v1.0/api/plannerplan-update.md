---
title: Atualizar plannerPlan
description: Atualize as propriedades do objeto **plannerPlan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 51fa3c1152d3442f1eff319d7f7cb112be53b063
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276528"
---
# <a name="update-plannerplan"></a><span data-ttu-id="84a5f-103">Atualizar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="84a5f-103">Update plannerPlan</span></span>

<span data-ttu-id="84a5f-104">Atualize as propriedades do objeto **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="84a5f-104">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84a5f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="84a5f-105">Permissions</span></span>
<span data-ttu-id="84a5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84a5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84a5f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84a5f-108">Permission type</span></span>      | <span data-ttu-id="84a5f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84a5f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84a5f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84a5f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84a5f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a5f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="84a5f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84a5f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84a5f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a5f-113">Not supported.</span></span>    |
|<span data-ttu-id="84a5f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84a5f-114">Application</span></span> | <span data-ttu-id="84a5f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a5f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84a5f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84a5f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84a5f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84a5f-117">Request headers</span></span>

| <span data-ttu-id="84a5f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="84a5f-118">Name</span></span>       | <span data-ttu-id="84a5f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a5f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="84a5f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="84a5f-120">Authorization</span></span>  | <span data-ttu-id="84a5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84a5f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84a5f-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="84a5f-123">If-Match</span></span>  | <span data-ttu-id="84a5f-124">Último valor de ETag conhecido para o plannerPlan a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="84a5f-124">Last known ETag value for the plannerPlan to be updated.</span></span> <span data-ttu-id="84a5f-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84a5f-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84a5f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84a5f-126">Request body</span></span>
<span data-ttu-id="84a5f-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="84a5f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="84a5f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84a5f-130">Property</span></span>     | <span data-ttu-id="84a5f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84a5f-131">Type</span></span>   |<span data-ttu-id="84a5f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a5f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84a5f-133">owner</span><span class="sxs-lookup"><span data-stu-id="84a5f-133">owner</span></span>|<span data-ttu-id="84a5f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a5f-134">String</span></span>|<span data-ttu-id="84a5f-135">[Grupo](../resources/group.md) `id` pelo qual o plano é proprietário.</span><span class="sxs-lookup"><span data-stu-id="84a5f-135">[Group](../resources/group.md) `id` by which the plan is owned.</span></span> <span data-ttu-id="84a5f-136">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="84a5f-136">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="84a5f-137">Uma vez definido, isso só pode ser atualizado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="84a5f-137">Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="84a5f-138">title</span><span class="sxs-lookup"><span data-stu-id="84a5f-138">title</span></span>|<span data-ttu-id="84a5f-139">String</span><span class="sxs-lookup"><span data-stu-id="84a5f-139">String</span></span>|<span data-ttu-id="84a5f-140">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="84a5f-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="84a5f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a5f-141">Response</span></span>

<span data-ttu-id="84a5f-142">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerPlan](../resources/plannerplan.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84a5f-142">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="84a5f-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="84a5f-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="84a5f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84a5f-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84a5f-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84a5f-147">Request</span></span>
<span data-ttu-id="84a5f-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84a5f-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="84a5f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a5f-149">Response</span></span>
<span data-ttu-id="84a5f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84a5f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84a5f-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="84a5f-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84a5f-154">C#</span><span class="sxs-lookup"><span data-stu-id="84a5f-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerplan-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84a5f-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="84a5f-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerplan-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="84a5f-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="84a5f-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_plannerplan-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplan-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/plannerplan-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplan-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
