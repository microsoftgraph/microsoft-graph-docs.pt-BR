---
title: Atualizar nameditem
description: Atualize as propriedades do objeto nameditem.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: b812058bcc7ce149b5a12b5c006e34c3f6368926
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052107"
---
# <a name="update-nameditem"></a><span data-ttu-id="a65e1-103">Atualizar nameditem</span><span class="sxs-lookup"><span data-stu-id="a65e1-103">Update nameditem</span></span>

<span data-ttu-id="a65e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a65e1-105">Atualize as propriedades do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="a65e1-105">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a65e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a65e1-106">Permissions</span></span>
<span data-ttu-id="a65e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a65e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a65e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a65e1-109">Permission type</span></span>      | <span data-ttu-id="a65e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a65e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a65e1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a65e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a65e1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a65e1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a65e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a65e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a65e1-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a65e1-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a65e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a65e1-115">Application</span></span> | <span data-ttu-id="a65e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a65e1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a65e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a65e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a65e1-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a65e1-118">Optional request headers</span></span>
| <span data-ttu-id="a65e1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a65e1-119">Name</span></span>       | <span data-ttu-id="a65e1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a65e1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a65e1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a65e1-121">Authorization</span></span>  | <span data-ttu-id="a65e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a65e1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a65e1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a65e1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a65e1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a65e1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a65e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a65e1-127">Request body</span></span>
<span data-ttu-id="a65e1-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a65e1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a65e1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a65e1-131">Property</span></span>     | <span data-ttu-id="a65e1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a65e1-132">Type</span></span>   |<span data-ttu-id="a65e1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a65e1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a65e1-134">visible</span><span class="sxs-lookup"><span data-stu-id="a65e1-134">visible</span></span>|<span data-ttu-id="a65e1-135">booliano</span><span class="sxs-lookup"><span data-stu-id="a65e1-135">boolean</span></span>|<span data-ttu-id="a65e1-136">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="a65e1-136">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="a65e1-137">comment</span><span class="sxs-lookup"><span data-stu-id="a65e1-137">comment</span></span>|   <span data-ttu-id="a65e1-138">string</span><span class="sxs-lookup"><span data-stu-id="a65e1-138">string</span></span>  |<span data-ttu-id="a65e1-139">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="a65e1-139">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="a65e1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a65e1-140">Response</span></span>

<span data-ttu-id="a65e1-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [workbookNamedItem](../resources/workbooknameditem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a65e1-141">If successful, this method returns a `200 OK` response code and updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a65e1-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a65e1-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a65e1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a65e1-143">Request</span></span>
<span data-ttu-id="a65e1-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a65e1-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a65e1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a65e1-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a65e1-146">C#</span><span class="sxs-lookup"><span data-stu-id="a65e1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a65e1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a65e1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a65e1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a65e1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a65e1-149">Java</span><span class="sxs-lookup"><span data-stu-id="a65e1-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-nameditem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a65e1-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a65e1-150">Response</span></span>
<span data-ttu-id="a65e1-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a65e1-151">Here is an example of the response.</span></span> <span data-ttu-id="a65e1-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a65e1-152">Note: The response object shown here might be shortened for readability.</span></span>
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


