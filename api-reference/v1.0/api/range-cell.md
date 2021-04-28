---
title: 'Range: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cb55594acc0b31ca9ce8f4f18d87df4f1529b2a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050357"
---
# <a name="range-cell"></a><span data-ttu-id="f9e3c-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="f9e3c-105">Range: Cell</span></span>

<span data-ttu-id="f9e3c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9e3c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9e3c-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9e3c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9e3c-110">Permissions</span></span>
<span data-ttu-id="f9e3c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9e3c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9e3c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9e3c-113">Permission type</span></span>      | <span data-ttu-id="f9e3c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9e3c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9e3c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9e3c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f9e3c-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9e3c-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9e3c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9e3c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9e3c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-118">Not supported.</span></span>    |
|<span data-ttu-id="f9e3c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9e3c-119">Application</span></span> | <span data-ttu-id="f9e3c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9e3c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9e3c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/cell
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/cell
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/cell
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="f9e3c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e3c-122">Request headers</span></span>
| <span data-ttu-id="f9e3c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f9e3c-123">Name</span></span>       | <span data-ttu-id="f9e3c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e3c-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9e3c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9e3c-125">Authorization</span></span>  | <span data-ttu-id="f9e3c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9e3c-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9e3c-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9e3c-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="f9e3c-131">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="f9e3c-131">Path parameters</span></span>
<span data-ttu-id="f9e3c-132">No caminho, forneça os parâmetros a seguir.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-132">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="f9e3c-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9e3c-133">Parameter</span></span>    | <span data-ttu-id="f9e3c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9e3c-134">Type</span></span>   |<span data-ttu-id="f9e3c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e3c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9e3c-136">row</span><span class="sxs-lookup"><span data-stu-id="f9e3c-136">row</span></span>|<span data-ttu-id="f9e3c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f9e3c-137">Int32</span></span>|<span data-ttu-id="f9e3c-p106">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="f9e3c-140">column</span><span class="sxs-lookup"><span data-stu-id="f9e3c-140">column</span></span>|<span data-ttu-id="f9e3c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f9e3c-141">Int32</span></span>|<span data-ttu-id="f9e3c-p107">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f9e3c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9e3c-144">Response</span></span>

<span data-ttu-id="f9e3c-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9e3c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9e3c-146">Example</span></span>
<span data-ttu-id="f9e3c-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9e3c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e3c-148">Request</span></span>
<span data-ttu-id="f9e3c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9e3c-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9e3c-150">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```
# <a name="c"></a>[<span data-ttu-id="f9e3c-151">C#</span><span class="sxs-lookup"><span data-stu-id="f9e3c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-cell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9e3c-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9e3c-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-cell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9e3c-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9e3c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-cell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9e3c-154">Java</span><span class="sxs-lookup"><span data-stu-id="f9e3c-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-cell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9e3c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9e3c-155">Response</span></span>
<span data-ttu-id="f9e3c-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-156">Here is an example of the response.</span></span> <span data-ttu-id="f9e3c-157">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9e3c-157">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

