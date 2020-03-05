---
title: 'Range: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 92c7b709a2e51431c4e5806e400030880c613e20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454791"
---
# <a name="range-cell"></a><span data-ttu-id="d2d7a-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="d2d7a-105">Range: Cell</span></span>

<span data-ttu-id="d2d7a-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2d7a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2d7a-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2d7a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2d7a-110">Permissions</span></span>
<span data-ttu-id="d2d7a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d7a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2d7a-113">Permission type</span></span>      | <span data-ttu-id="d2d7a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2d7a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2d7a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2d7a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d2d7a-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2d7a-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2d7a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2d7a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d7a-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2d7a-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2d7a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2d7a-119">Application</span></span> | <span data-ttu-id="d2d7a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2d7a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2d7a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="d2d7a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2d7a-122">Request headers</span></span>
| <span data-ttu-id="d2d7a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d2d7a-123">Name</span></span>       | <span data-ttu-id="d2d7a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2d7a-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2d7a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2d7a-125">Authorization</span></span>  | <span data-ttu-id="d2d7a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2d7a-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2d7a-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2d7a-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d7a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2d7a-131">Request body</span></span>
<span data-ttu-id="d2d7a-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2d7a-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d2d7a-133">Parameter</span></span>    | <span data-ttu-id="d2d7a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2d7a-134">Type</span></span>   |<span data-ttu-id="d2d7a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2d7a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2d7a-136">row</span><span class="sxs-lookup"><span data-stu-id="d2d7a-136">row</span></span>|<span data-ttu-id="d2d7a-137">number</span><span class="sxs-lookup"><span data-stu-id="d2d7a-137">number</span></span>|<span data-ttu-id="d2d7a-p106">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="d2d7a-140">column</span><span class="sxs-lookup"><span data-stu-id="d2d7a-140">column</span></span>|<span data-ttu-id="d2d7a-141">número</span><span class="sxs-lookup"><span data-stu-id="d2d7a-141">number</span></span>|<span data-ttu-id="d2d7a-p107">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="d2d7a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2d7a-144">Response</span></span>

<span data-ttu-id="d2d7a-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d7a-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2d7a-146">Example</span></span>
<span data-ttu-id="d2d7a-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2d7a-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2d7a-148">Request</span></span>
<span data-ttu-id="d2d7a-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="d2d7a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2d7a-150">Response</span></span>
<span data-ttu-id="d2d7a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2d7a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
