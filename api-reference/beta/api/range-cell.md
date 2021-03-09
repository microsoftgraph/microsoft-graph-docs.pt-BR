---
title: 'Range: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 491313183aa29b3acb38b3e9003ac7dc06bf819a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575991"
---
# <a name="range-cell"></a><span data-ttu-id="a933e-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="a933e-105">Range: Cell</span></span>

<span data-ttu-id="a933e-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a933e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a933e-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="a933e-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="a933e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a933e-110">Permissions</span></span>
<span data-ttu-id="a933e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a933e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a933e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a933e-113">Permission type</span></span>      | <span data-ttu-id="a933e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a933e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a933e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a933e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a933e-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a933e-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a933e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a933e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a933e-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a933e-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a933e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a933e-119">Application</span></span> | <span data-ttu-id="a933e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a933e-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a933e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a933e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/Cell
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/Cell
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Cell
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="a933e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a933e-122">Request headers</span></span>
| <span data-ttu-id="a933e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a933e-123">Name</span></span>       | <span data-ttu-id="a933e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a933e-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a933e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a933e-125">Authorization</span></span>  | <span data-ttu-id="a933e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a933e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a933e-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a933e-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="a933e-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a933e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a933e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a933e-131">Request body</span></span>
<span data-ttu-id="a933e-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a933e-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a933e-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a933e-133">Parameter</span></span>    | <span data-ttu-id="a933e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a933e-134">Type</span></span>   |<span data-ttu-id="a933e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a933e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a933e-136">row</span><span class="sxs-lookup"><span data-stu-id="a933e-136">row</span></span>|<span data-ttu-id="a933e-137">number</span><span class="sxs-lookup"><span data-stu-id="a933e-137">number</span></span>|<span data-ttu-id="a933e-p106">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="a933e-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="a933e-140">column</span><span class="sxs-lookup"><span data-stu-id="a933e-140">column</span></span>|<span data-ttu-id="a933e-141">number</span><span class="sxs-lookup"><span data-stu-id="a933e-141">number</span></span>|<span data-ttu-id="a933e-p107">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="a933e-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a933e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a933e-144">Response</span></span>

<span data-ttu-id="a933e-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a933e-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a933e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a933e-146">Example</span></span>
<span data-ttu-id="a933e-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a933e-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a933e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a933e-148">Request</span></span>
<span data-ttu-id="a933e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a933e-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a933e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a933e-150">Response</span></span>
<span data-ttu-id="a933e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a933e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


