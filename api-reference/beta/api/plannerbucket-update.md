---
title: Atualizar plannerbucket
description: Atualize as propriedades do objeto **plannerbucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a041df5f7acf26a5e8df2a8d050e7f27d3b5d8a4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349478"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="63bd2-103">Atualizar plannerbucket</span><span class="sxs-lookup"><span data-stu-id="63bd2-103">Update plannerbucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63bd2-104">Atualize as propriedades do objeto **plannerbucket** .</span><span class="sxs-lookup"><span data-stu-id="63bd2-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="63bd2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="63bd2-105">Permissions</span></span>
<span data-ttu-id="63bd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63bd2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63bd2-108">Permission type</span></span>      | <span data-ttu-id="63bd2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63bd2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63bd2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63bd2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63bd2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bd2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63bd2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63bd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63bd2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63bd2-113">Not supported.</span></span>    |
|<span data-ttu-id="63bd2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63bd2-114">Application</span></span> | <span data-ttu-id="63bd2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63bd2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63bd2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63bd2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="63bd2-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="63bd2-117">Optional request headers</span></span>
| <span data-ttu-id="63bd2-118">Name</span><span class="sxs-lookup"><span data-stu-id="63bd2-118">Name</span></span>       | <span data-ttu-id="63bd2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="63bd2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="63bd2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="63bd2-120">Authorization</span></span>  | <span data-ttu-id="63bd2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63bd2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63bd2-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="63bd2-123">If-Match</span></span>  | <span data-ttu-id="63bd2-124">Último valor de ETag conhecido para o **plannerBucket** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="63bd2-124">Last known ETag value for the **plannerBucket** to be updated.</span></span> <span data-ttu-id="63bd2-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63bd2-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63bd2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63bd2-126">Request body</span></span>
<span data-ttu-id="63bd2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="63bd2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63bd2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63bd2-130">Property</span></span>     | <span data-ttu-id="63bd2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63bd2-131">Type</span></span>   |<span data-ttu-id="63bd2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63bd2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63bd2-133">name</span><span class="sxs-lookup"><span data-stu-id="63bd2-133">name</span></span>|<span data-ttu-id="63bd2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63bd2-134">String</span></span>|<span data-ttu-id="63bd2-135">Nome do Bucket.</span><span class="sxs-lookup"><span data-stu-id="63bd2-135">Name of the bucket.</span></span>|
|<span data-ttu-id="63bd2-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="63bd2-136">orderHint</span></span>|<span data-ttu-id="63bd2-137">String</span><span class="sxs-lookup"><span data-stu-id="63bd2-137">String</span></span>|<span data-ttu-id="63bd2-138">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="63bd2-138">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="63bd2-139">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="63bd2-139">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="63bd2-140">planId</span><span class="sxs-lookup"><span data-stu-id="63bd2-140">planId</span></span>|<span data-ttu-id="63bd2-141">String</span><span class="sxs-lookup"><span data-stu-id="63bd2-141">String</span></span>|<span data-ttu-id="63bd2-142">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="63bd2-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="63bd2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bd2-143">Response</span></span>

<span data-ttu-id="63bd2-144">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucket](../resources/plannerbucket.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63bd2-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="63bd2-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="63bd2-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="63bd2-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63bd2-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63bd2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63bd2-149">Request</span></span>
<span data-ttu-id="63bd2-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63bd2-150">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63bd2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="63bd2-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="63bd2-152">C#</span><span class="sxs-lookup"><span data-stu-id="63bd2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63bd2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63bd2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63bd2-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="63bd2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="63bd2-155">Java</span><span class="sxs-lookup"><span data-stu-id="63bd2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63bd2-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bd2-156">Response</span></span>
<span data-ttu-id="63bd2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63bd2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
