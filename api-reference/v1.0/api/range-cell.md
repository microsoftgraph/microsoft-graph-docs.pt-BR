---
title: 'Range: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 0c9eac781fbe836cff1c4a0576c6da87d847b3ec
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607695"
---
# <a name="range-cell"></a><span data-ttu-id="b90d7-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="b90d7-105">Range: Cell</span></span>

<span data-ttu-id="b90d7-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="b90d7-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="b90d7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b90d7-109">Permissions</span></span>
<span data-ttu-id="b90d7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b90d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b90d7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b90d7-112">Permission type</span></span>      | <span data-ttu-id="b90d7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b90d7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b90d7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b90d7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b90d7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b90d7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b90d7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b90d7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b90d7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b90d7-117">Not supported.</span></span>    |
|<span data-ttu-id="b90d7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b90d7-118">Application</span></span> | <span data-ttu-id="b90d7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b90d7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b90d7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b90d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="b90d7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b90d7-121">Request headers</span></span>
| <span data-ttu-id="b90d7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b90d7-122">Name</span></span>       | <span data-ttu-id="b90d7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b90d7-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b90d7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b90d7-124">Authorization</span></span>  | <span data-ttu-id="b90d7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b90d7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b90d7-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b90d7-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="b90d7-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b90d7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="b90d7-130">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="b90d7-130">Path parameters</span></span>
<span data-ttu-id="b90d7-131">No caminho, forneça os parâmetros a seguir.</span><span class="sxs-lookup"><span data-stu-id="b90d7-131">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="b90d7-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b90d7-132">Parameter</span></span>    | <span data-ttu-id="b90d7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b90d7-133">Type</span></span>   |<span data-ttu-id="b90d7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b90d7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b90d7-135">row</span><span class="sxs-lookup"><span data-stu-id="b90d7-135">row</span></span>|<span data-ttu-id="b90d7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b90d7-136">Int32</span></span>|<span data-ttu-id="b90d7-p106">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="b90d7-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="b90d7-139">column</span><span class="sxs-lookup"><span data-stu-id="b90d7-139">column</span></span>|<span data-ttu-id="b90d7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b90d7-140">Int32</span></span>|<span data-ttu-id="b90d7-p107">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="b90d7-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="b90d7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b90d7-143">Response</span></span>

<span data-ttu-id="b90d7-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b90d7-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b90d7-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b90d7-145">Example</span></span>
<span data-ttu-id="b90d7-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b90d7-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b90d7-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b90d7-147">Request</span></span>
<span data-ttu-id="b90d7-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b90d7-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```

##### <a name="response"></a><span data-ttu-id="b90d7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b90d7-149">Response</span></span>
<span data-ttu-id="b90d7-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b90d7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b90d7-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b90d7-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b90d7-154">Basic</span><span class="sxs-lookup"><span data-stu-id="b90d7-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_cell-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b90d7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b90d7-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_cell-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-cell.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-cell.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
