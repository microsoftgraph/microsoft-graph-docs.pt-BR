---
title: Atualizar nameditem
description: Atualize as propriedades do objeto nameditem.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 940502c48db07cc39753366a2d5714e1c3b2d7b5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414816"
---
# <a name="update-nameditem"></a><span data-ttu-id="6ce74-103">Atualizar nameditem</span><span class="sxs-lookup"><span data-stu-id="6ce74-103">Update nameditem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ce74-104">Atualize as propriedades do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="6ce74-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ce74-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ce74-105">Permissions</span></span>
<span data-ttu-id="6ce74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ce74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce74-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ce74-108">Permission type</span></span>      | <span data-ttu-id="6ce74-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ce74-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ce74-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ce74-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ce74-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ce74-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ce74-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ce74-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ce74-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ce74-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ce74-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ce74-114">Application</span></span> | <span data-ttu-id="6ce74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ce74-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ce74-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ce74-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="6ce74-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6ce74-117">Optional request headers</span></span>
| <span data-ttu-id="6ce74-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6ce74-118">Name</span></span>       | <span data-ttu-id="6ce74-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ce74-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6ce74-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ce74-120">Authorization</span></span>  | <span data-ttu-id="6ce74-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ce74-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ce74-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ce74-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ce74-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6ce74-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce74-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce74-126">Request body</span></span>
<span data-ttu-id="6ce74-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6ce74-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6ce74-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ce74-130">Property</span></span>     | <span data-ttu-id="6ce74-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ce74-131">Type</span></span>   |<span data-ttu-id="6ce74-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ce74-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ce74-133">visible</span><span class="sxs-lookup"><span data-stu-id="6ce74-133">visible</span></span>|<span data-ttu-id="6ce74-134">booliano</span><span class="sxs-lookup"><span data-stu-id="6ce74-134">boolean</span></span>|<span data-ttu-id="6ce74-135">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="6ce74-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="6ce74-136">comment</span><span class="sxs-lookup"><span data-stu-id="6ce74-136">comment</span></span>|   <span data-ttu-id="6ce74-137">string</span><span class="sxs-lookup"><span data-stu-id="6ce74-137">string</span></span>  |<span data-ttu-id="6ce74-138">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="6ce74-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="6ce74-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce74-139">Response</span></span>

<span data-ttu-id="6ce74-140">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookNamedItem](../resources/workbooknameditem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ce74-140">If successful, this method returns a `200 OK` response code and updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ce74-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ce74-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ce74-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce74-142">Request</span></span>
<span data-ttu-id="6ce74-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ce74-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ce74-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ce74-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ce74-145">C#</span><span class="sxs-lookup"><span data-stu-id="6ce74-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ce74-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ce74-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ce74-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6ce74-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ce74-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce74-148">Response</span></span>
<span data-ttu-id="6ce74-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ce74-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
