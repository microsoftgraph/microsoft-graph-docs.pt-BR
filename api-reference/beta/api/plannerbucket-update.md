---
title: Atualizar plannerbucket
description: Atualize as propriedades do objeto **plannerbucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 87b722ce97a2d90afa4b298ab445516b58a56a7e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268317"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="703f4-103">Atualizar plannerbucket</span><span class="sxs-lookup"><span data-stu-id="703f4-103">Update plannerbucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="703f4-104">Atualize as propriedades do objeto **plannerbucket** .</span><span class="sxs-lookup"><span data-stu-id="703f4-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="703f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="703f4-105">Permissions</span></span>
<span data-ttu-id="703f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="703f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="703f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="703f4-108">Permission type</span></span>      | <span data-ttu-id="703f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="703f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="703f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="703f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="703f4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703f4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="703f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="703f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="703f4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="703f4-113">Not supported.</span></span>    |
|<span data-ttu-id="703f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="703f4-114">Application</span></span> | <span data-ttu-id="703f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="703f4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="703f4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="703f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="703f4-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="703f4-117">Optional request headers</span></span>
| <span data-ttu-id="703f4-118">Name</span><span class="sxs-lookup"><span data-stu-id="703f4-118">Name</span></span>       | <span data-ttu-id="703f4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="703f4-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="703f4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="703f4-120">Authorization</span></span>  | <span data-ttu-id="703f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="703f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="703f4-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="703f4-123">If-Match</span></span>  | <span data-ttu-id="703f4-124">Último valor de ETag conhecido para o **plannerBucket** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="703f4-124">Last known ETag value for the **plannerBucket** to be updated.</span></span> <span data-ttu-id="703f4-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="703f4-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="703f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="703f4-126">Request body</span></span>
<span data-ttu-id="703f4-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="703f4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="703f4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="703f4-130">Property</span></span>     | <span data-ttu-id="703f4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="703f4-131">Type</span></span>   |<span data-ttu-id="703f4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="703f4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="703f4-133">name</span><span class="sxs-lookup"><span data-stu-id="703f4-133">name</span></span>|<span data-ttu-id="703f4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f4-134">String</span></span>|<span data-ttu-id="703f4-135">Nome do Bucket.</span><span class="sxs-lookup"><span data-stu-id="703f4-135">Name of the bucket.</span></span>|
|<span data-ttu-id="703f4-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="703f4-136">orderHint</span></span>|<span data-ttu-id="703f4-137">String</span><span class="sxs-lookup"><span data-stu-id="703f4-137">String</span></span>|<span data-ttu-id="703f4-138">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="703f4-138">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="703f4-139">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="703f4-139">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="703f4-140">planId</span><span class="sxs-lookup"><span data-stu-id="703f4-140">planId</span></span>|<span data-ttu-id="703f4-141">String</span><span class="sxs-lookup"><span data-stu-id="703f4-141">String</span></span>|<span data-ttu-id="703f4-142">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="703f4-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="703f4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="703f4-143">Response</span></span>

<span data-ttu-id="703f4-144">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucket](../resources/plannerbucket.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="703f4-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="703f4-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="703f4-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="703f4-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="703f4-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="703f4-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="703f4-149">Request</span></span>
<span data-ttu-id="703f4-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="703f4-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="703f4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="703f4-151">Response</span></span>
<span data-ttu-id="703f4-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="703f4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="703f4-155">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="703f4-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="703f4-156">C#</span><span class="sxs-lookup"><span data-stu-id="703f4-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerbucket-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="703f4-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="703f4-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerbucket-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="703f4-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="703f4-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_plannerbucket-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbucket-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannerbucket-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerbucket-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
