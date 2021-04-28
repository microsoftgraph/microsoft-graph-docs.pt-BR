---
title: Adicionar item nomeado FormulaLocal
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 95b1733b0d3c281ca9a1e96d0d484a4ba2a2e1d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055901"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="b62f9-103">Adicionar item nomeado FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="b62f9-103">Add Named Item FormulaLocal</span></span>

<span data-ttu-id="b62f9-104">Namespace: microsoft.graph Adiciona um novo nome à coleção do escopo determinado usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="b62f9-104">Namespace: microsoft.graph Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="b62f9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b62f9-105">Permissions</span></span>
<span data-ttu-id="b62f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b62f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b62f9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b62f9-108">Permission type</span></span>      | <span data-ttu-id="b62f9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b62f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b62f9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b62f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b62f9-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="b62f9-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="b62f9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b62f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b62f9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b62f9-113">Not supported.</span></span>    |
|<span data-ttu-id="b62f9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b62f9-114">Application</span></span> | <span data-ttu-id="b62f9-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="b62f9-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b62f9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b62f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/add
POST /me/drive/root:/{item-path}:/workbook/names/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/names/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/names/add

```
## <a name="request-headers"></a><span data-ttu-id="b62f9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b62f9-117">Request headers</span></span>
| <span data-ttu-id="b62f9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b62f9-118">Name</span></span>       | <span data-ttu-id="b62f9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b62f9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b62f9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b62f9-120">Authorization</span></span>  | <span data-ttu-id="b62f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b62f9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b62f9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b62f9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b62f9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b62f9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b62f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b62f9-126">Request body</span></span>
<span data-ttu-id="b62f9-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b62f9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b62f9-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b62f9-128">Parameter</span></span>    | <span data-ttu-id="b62f9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b62f9-129">Type</span></span>   |<span data-ttu-id="b62f9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b62f9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b62f9-131">nome</span><span class="sxs-lookup"><span data-stu-id="b62f9-131">name</span></span>|<span data-ttu-id="b62f9-132">string</span><span class="sxs-lookup"><span data-stu-id="b62f9-132">string</span></span>|<span data-ttu-id="b62f9-133">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="b62f9-133">The name of the named item.</span></span>|
|<span data-ttu-id="b62f9-134">formula</span><span class="sxs-lookup"><span data-stu-id="b62f9-134">formula</span></span>|<span data-ttu-id="b62f9-135">string</span><span class="sxs-lookup"><span data-stu-id="b62f9-135">string</span></span>|<span data-ttu-id="b62f9-136">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="b62f9-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="b62f9-137">comment</span><span class="sxs-lookup"><span data-stu-id="b62f9-137">comment</span></span>|<span data-ttu-id="b62f9-138">string</span><span class="sxs-lookup"><span data-stu-id="b62f9-138">string</span></span>|<span data-ttu-id="b62f9-139">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="b62f9-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="b62f9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b62f9-140">Response</span></span>

<span data-ttu-id="b62f9-141">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookNamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b62f9-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b62f9-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b62f9-142">Example</span></span>
<span data-ttu-id="b62f9-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b62f9-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b62f9-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b62f9-144">Request</span></span>
<span data-ttu-id="b62f9-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b62f9-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b62f9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b62f9-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```
# <a name="c"></a>[<span data-ttu-id="b62f9-147">C#</span><span class="sxs-lookup"><span data-stu-id="b62f9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b62f9-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b62f9-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b62f9-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b62f9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b62f9-150">Java</span><span class="sxs-lookup"><span data-stu-id="b62f9-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b62f9-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b62f9-151">Response</span></span>
<span data-ttu-id="b62f9-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b62f9-152">Here is an example of the response.</span></span> <span data-ttu-id="b62f9-153">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b62f9-153">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

