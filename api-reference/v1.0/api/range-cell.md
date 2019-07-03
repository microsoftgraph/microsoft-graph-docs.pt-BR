---
title: 'Range: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 493bc206e3a4833ad12b7733bcfb5abf92d89e81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448567"
---
# <a name="range-cell"></a><span data-ttu-id="44205-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="44205-105">Range: Cell</span></span>

<span data-ttu-id="44205-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="44205-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="44205-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="44205-109">Permissions</span></span>
<span data-ttu-id="44205-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44205-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44205-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44205-112">Permission type</span></span>      | <span data-ttu-id="44205-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44205-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44205-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44205-114">Delegated (work or school account)</span></span> | <span data-ttu-id="44205-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44205-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44205-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44205-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44205-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44205-117">Not supported.</span></span>    |
|<span data-ttu-id="44205-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44205-118">Application</span></span> | <span data-ttu-id="44205-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44205-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44205-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44205-120">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44205-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="44205-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="44205-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44205-122">Request headers</span></span>
| <span data-ttu-id="44205-123">Nome</span><span class="sxs-lookup"><span data-stu-id="44205-123">Name</span></span>       | <span data-ttu-id="44205-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="44205-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44205-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="44205-125">Authorization</span></span>  | <span data-ttu-id="44205-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44205-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44205-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44205-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="44205-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="44205-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="44205-131">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="44205-131">Path parameters</span></span>
<span data-ttu-id="44205-132">No caminho, forneça os parâmetros a seguir.</span><span class="sxs-lookup"><span data-stu-id="44205-132">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="44205-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="44205-133">Parameter</span></span>    | <span data-ttu-id="44205-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="44205-134">Type</span></span>   |<span data-ttu-id="44205-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="44205-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44205-136">row</span><span class="sxs-lookup"><span data-stu-id="44205-136">row</span></span>|<span data-ttu-id="44205-137">Int32</span><span class="sxs-lookup"><span data-stu-id="44205-137">Int32</span></span>|<span data-ttu-id="44205-p106">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="44205-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="44205-140">column</span><span class="sxs-lookup"><span data-stu-id="44205-140">column</span></span>|<span data-ttu-id="44205-141">Int32</span><span class="sxs-lookup"><span data-stu-id="44205-141">Int32</span></span>|<span data-ttu-id="44205-p107">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="44205-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="44205-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="44205-144">Response</span></span>

<span data-ttu-id="44205-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44205-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44205-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44205-146">Example</span></span>
<span data-ttu-id="44205-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="44205-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44205-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44205-148">Request</span></span>
<span data-ttu-id="44205-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44205-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44205-150">C#</span><span class="sxs-lookup"><span data-stu-id="44205-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-cell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44205-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="44205-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-cell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44205-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="44205-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-cell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="44205-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="44205-153">Response</span></span>
<span data-ttu-id="44205-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44205-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
