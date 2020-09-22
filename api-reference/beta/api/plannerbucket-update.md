---
title: Atualizar plannerbucket
description: Atualize as propriedades do objeto **plannerbucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 2879c82946e308644893e4ed4015d2e2705d6854
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085574"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="0c66a-103">Atualizar plannerbucket</span><span class="sxs-lookup"><span data-stu-id="0c66a-103">Update plannerbucket</span></span>

<span data-ttu-id="0c66a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c66a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c66a-105">Atualize as propriedades do objeto **plannerbucket** .</span><span class="sxs-lookup"><span data-stu-id="0c66a-105">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c66a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c66a-106">Permissions</span></span>
<span data-ttu-id="0c66a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c66a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c66a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c66a-109">Permission type</span></span>      | <span data-ttu-id="0c66a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c66a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c66a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c66a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0c66a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c66a-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c66a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c66a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c66a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c66a-114">Not supported.</span></span>    |
|<span data-ttu-id="0c66a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c66a-115">Application</span></span> | <span data-ttu-id="0c66a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c66a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c66a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c66a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0c66a-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0c66a-118">Optional request headers</span></span>
| <span data-ttu-id="0c66a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0c66a-119">Name</span></span>       | <span data-ttu-id="0c66a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c66a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0c66a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c66a-121">Authorization</span></span>  | <span data-ttu-id="0c66a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c66a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c66a-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="0c66a-124">If-Match</span></span>  | <span data-ttu-id="0c66a-125">Último valor de ETag conhecido para o **plannerBucket** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="0c66a-125">Last known ETag value for the **plannerBucket** to be updated.</span></span> <span data-ttu-id="0c66a-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c66a-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c66a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c66a-127">Request body</span></span>
<span data-ttu-id="0c66a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0c66a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c66a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c66a-131">Property</span></span>     | <span data-ttu-id="0c66a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c66a-132">Type</span></span>   |<span data-ttu-id="0c66a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c66a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c66a-134">name</span><span class="sxs-lookup"><span data-stu-id="0c66a-134">name</span></span>|<span data-ttu-id="0c66a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c66a-135">String</span></span>|<span data-ttu-id="0c66a-136">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="0c66a-136">Name of the bucket.</span></span>|
|<span data-ttu-id="0c66a-137">orderHint</span><span class="sxs-lookup"><span data-stu-id="0c66a-137">orderHint</span></span>|<span data-ttu-id="0c66a-138">String</span><span class="sxs-lookup"><span data-stu-id="0c66a-138">String</span></span>|<span data-ttu-id="0c66a-139">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="0c66a-139">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="0c66a-140">O formato é definido em [usando dicas de ordenação no Planner](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="0c66a-140">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="0c66a-141">planId</span><span class="sxs-lookup"><span data-stu-id="0c66a-141">planId</span></span>|<span data-ttu-id="0c66a-142">String</span><span class="sxs-lookup"><span data-stu-id="0c66a-142">String</span></span>|<span data-ttu-id="0c66a-143">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="0c66a-143">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="0c66a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c66a-144">Response</span></span>

<span data-ttu-id="0c66a-145">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucket](../resources/plannerbucket.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c66a-145">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="0c66a-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0c66a-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0c66a-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c66a-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c66a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c66a-150">Request</span></span>
<span data-ttu-id="0c66a-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c66a-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c66a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c66a-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0c66a-153">C#</span><span class="sxs-lookup"><span data-stu-id="0c66a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c66a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c66a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c66a-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c66a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0c66a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c66a-156">Response</span></span>
<span data-ttu-id="0c66a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c66a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


