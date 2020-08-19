---
title: Atualizar nameditem
description: Atualize as propriedades do objeto nameditem.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f75d034c7f4e5a6e3c8463e21114fc6a6a429a65
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809270"
---
# <a name="update-nameditem"></a><span data-ttu-id="6c8cc-103">Atualizar nameditem</span><span class="sxs-lookup"><span data-stu-id="6c8cc-103">Update nameditem</span></span>

<span data-ttu-id="6c8cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c8cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c8cc-105">Atualize as propriedades do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-105">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c8cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c8cc-106">Permissions</span></span>
<span data-ttu-id="6c8cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c8cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c8cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c8cc-109">Permission type</span></span>      | <span data-ttu-id="6c8cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c8cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c8cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c8cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6c8cc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c8cc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c8cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c8cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c8cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-114">Not supported.</span></span>    |
|<span data-ttu-id="6c8cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c8cc-115">Application</span></span> | <span data-ttu-id="6c8cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c8cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c8cc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="6c8cc-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6c8cc-118">Optional request headers</span></span>
| <span data-ttu-id="6c8cc-119">Name</span><span class="sxs-lookup"><span data-stu-id="6c8cc-119">Name</span></span>       | <span data-ttu-id="6c8cc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8cc-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6c8cc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c8cc-121">Authorization</span></span>  | <span data-ttu-id="6c8cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c8cc-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c8cc-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c8cc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c8cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8cc-127">Request body</span></span>
<span data-ttu-id="6c8cc-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6c8cc-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c8cc-131">Property</span></span>     | <span data-ttu-id="6c8cc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c8cc-132">Type</span></span>   |<span data-ttu-id="6c8cc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8cc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c8cc-134">visible</span><span class="sxs-lookup"><span data-stu-id="6c8cc-134">visible</span></span>|<span data-ttu-id="6c8cc-135">booliano</span><span class="sxs-lookup"><span data-stu-id="6c8cc-135">boolean</span></span>|<span data-ttu-id="6c8cc-136">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-136">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="6c8cc-137">comment</span><span class="sxs-lookup"><span data-stu-id="6c8cc-137">comment</span></span>|   <span data-ttu-id="6c8cc-138">string</span><span class="sxs-lookup"><span data-stu-id="6c8cc-138">string</span></span>  |<span data-ttu-id="6c8cc-139">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-139">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="6c8cc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c8cc-140">Response</span></span>

<span data-ttu-id="6c8cc-141">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookNamedItem](../resources/nameditem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-141">If successful, this method returns a `200 OK` response code and updated [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c8cc-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c8cc-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c8cc-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8cc-143">Request</span></span>
<span data-ttu-id="6c8cc-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c8cc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c8cc-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6c8cc-146">C#</span><span class="sxs-lookup"><span data-stu-id="6c8cc-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c8cc-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c8cc-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c8cc-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c8cc-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c8cc-149">Java</span><span class="sxs-lookup"><span data-stu-id="6c8cc-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-nameditem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6c8cc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c8cc-150">Response</span></span>
<span data-ttu-id="6c8cc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c8cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
