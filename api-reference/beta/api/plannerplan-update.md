---
title: Atualizar plannerPlan
description: Atualiza as propriedades de um objeto **plannerPlan** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 32a413538c1ebc6e4381b29b3220330e4637a95a
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820728"
---
# <a name="update-plannerplan"></a><span data-ttu-id="93512-103">Atualizar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="93512-103">Update plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93512-104">Atualiza as propriedades de um objeto **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="93512-104">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93512-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="93512-105">Permissions</span></span>
<span data-ttu-id="93512-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93512-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93512-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93512-108">Permission type</span></span>      | <span data-ttu-id="93512-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93512-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93512-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93512-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93512-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93512-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93512-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93512-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93512-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93512-113">Not supported.</span></span>    |
|<span data-ttu-id="93512-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93512-114">Application</span></span> | <span data-ttu-id="93512-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93512-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93512-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93512-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="93512-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93512-117">Request headers</span></span>

| <span data-ttu-id="93512-118">Nome</span><span class="sxs-lookup"><span data-stu-id="93512-118">Name</span></span>       | <span data-ttu-id="93512-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="93512-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="93512-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="93512-120">Authorization</span></span>  | <span data-ttu-id="93512-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93512-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93512-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="93512-123">If-Match</span></span>  | <span data-ttu-id="93512-124">Último valor de ETag conhecido para o plannerPlan a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="93512-124">Last known ETag value for the plannerPlan to be updated.</span></span> <span data-ttu-id="93512-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93512-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93512-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93512-126">Request body</span></span>
<span data-ttu-id="93512-127">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="93512-127">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="93512-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="93512-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="93512-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="93512-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="93512-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93512-130">Property</span></span>     | <span data-ttu-id="93512-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93512-131">Type</span></span>   |<span data-ttu-id="93512-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93512-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93512-133">owner</span><span class="sxs-lookup"><span data-stu-id="93512-133">owner</span></span>|<span data-ttu-id="93512-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93512-134">String</span></span>|<span data-ttu-id="93512-135">[Grupo](../resources/group.md) `id` pelo qual o plano é proprietário.</span><span class="sxs-lookup"><span data-stu-id="93512-135">[Group](../resources/group.md) `id` by which the plan is owned.</span></span> <span data-ttu-id="93512-136">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="93512-136">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="93512-137">Uma vez definido, isso só pode ser atualizado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="93512-137">Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="93512-138">title</span><span class="sxs-lookup"><span data-stu-id="93512-138">title</span></span>|<span data-ttu-id="93512-139">String</span><span class="sxs-lookup"><span data-stu-id="93512-139">String</span></span>|<span data-ttu-id="93512-140">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="93512-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="93512-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="93512-141">Response</span></span>

<span data-ttu-id="93512-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [plannerPlan](../resources/plannerplan.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93512-142">If successful, this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="93512-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="93512-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="93512-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93512-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93512-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93512-147">Request</span></span>
<span data-ttu-id="93512-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93512-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="93512-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="93512-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/<id>
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93512-150">C#</span><span class="sxs-lookup"><span data-stu-id="93512-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93512-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="93512-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93512-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="93512-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93512-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="93512-153">Response</span></span>
<span data-ttu-id="93512-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93512-154">Here is an example of the response.</span></span> 

><span data-ttu-id="93512-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93512-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
