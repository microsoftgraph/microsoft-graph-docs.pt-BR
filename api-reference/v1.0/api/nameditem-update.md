---
title: Atualizar nameditem
description: Atualize as propriedades do objeto nameditem.
localization_priority: Normal
ms.openlocfilehash: ad7f899791d64d5d3ef431d8875cba6fbcd150c0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890229"
---
# <a name="update-nameditem"></a><span data-ttu-id="0b651-103">Atualizar nameditem</span><span class="sxs-lookup"><span data-stu-id="0b651-103">Update nameditem</span></span>

<span data-ttu-id="0b651-104">Atualize as propriedades do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="0b651-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b651-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b651-105">Permissions</span></span>
<span data-ttu-id="0b651-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b651-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b651-108">Permission type</span></span>      | <span data-ttu-id="0b651-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b651-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b651-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b651-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b651-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b651-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b651-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b651-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b651-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b651-113">Not supported.</span></span>    |
|<span data-ttu-id="0b651-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b651-114">Application</span></span> | <span data-ttu-id="0b651-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b651-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b651-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b651-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0b651-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0b651-117">Optional request headers</span></span>
| <span data-ttu-id="0b651-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0b651-118">Name</span></span>       | <span data-ttu-id="0b651-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b651-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b651-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b651-120">Authorization</span></span>  | <span data-ttu-id="0b651-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b651-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b651-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b651-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b651-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0b651-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b651-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b651-126">Request body</span></span>
<span data-ttu-id="0b651-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0b651-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b651-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b651-130">Property</span></span>     | <span data-ttu-id="0b651-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b651-131">Type</span></span>   |<span data-ttu-id="0b651-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b651-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b651-133">visible</span><span class="sxs-lookup"><span data-stu-id="0b651-133">visible</span></span>|<span data-ttu-id="0b651-134">booliano</span><span class="sxs-lookup"><span data-stu-id="0b651-134">boolean</span></span>|<span data-ttu-id="0b651-135">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="0b651-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="0b651-136">comment</span><span class="sxs-lookup"><span data-stu-id="0b651-136">comment</span></span>|   <span data-ttu-id="0b651-137">string</span><span class="sxs-lookup"><span data-stu-id="0b651-137">string</span></span>  |<span data-ttu-id="0b651-138">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="0b651-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="0b651-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b651-139">Response</span></span>

<span data-ttu-id="0b651-140">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookNamedItem](../resources/nameditem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b651-140">If successful, this method returns a `200 OK` response code and updated [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b651-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b651-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b651-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b651-142">Request</span></span>
<span data-ttu-id="0b651-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b651-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b651-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b651-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b651-145">C#</span><span class="sxs-lookup"><span data-stu-id="0b651-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b651-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b651-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b651-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b651-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b651-148">Java</span><span class="sxs-lookup"><span data-stu-id="0b651-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-nameditem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b651-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b651-149">Response</span></span>
<span data-ttu-id="0b651-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b651-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
