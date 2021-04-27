---
title: 'Worksheet: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2a5d5d108974f337d74788ddec2b3fdc05f9d3f1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051666"
---
# <a name="worksheet-cell"></a><span data-ttu-id="23ae7-104">Planilha: Célula</span><span class="sxs-lookup"><span data-stu-id="23ae7-104">Worksheet: Cell</span></span>

<span data-ttu-id="23ae7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ae7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ae7-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="23ae7-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="23ae7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="23ae7-108">Permissions</span></span>
<span data-ttu-id="23ae7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ae7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ae7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23ae7-111">Permission type</span></span>      | <span data-ttu-id="23ae7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23ae7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23ae7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23ae7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="23ae7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ae7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23ae7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23ae7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ae7-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ae7-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23ae7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23ae7-117">Application</span></span> | <span data-ttu-id="23ae7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23ae7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23ae7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23ae7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row={row},column={column})
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="23ae7-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="23ae7-120">Function parameters</span></span>
<span data-ttu-id="23ae7-121">No caminho da solicitação, forneça os parâmetros a seguir.</span><span class="sxs-lookup"><span data-stu-id="23ae7-121">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="23ae7-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="23ae7-122">Parameter</span></span>    | <span data-ttu-id="23ae7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="23ae7-123">Type</span></span>   |<span data-ttu-id="23ae7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ae7-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23ae7-125">row</span><span class="sxs-lookup"><span data-stu-id="23ae7-125">row</span></span>|<span data-ttu-id="23ae7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="23ae7-126">Int32</span></span>|<span data-ttu-id="23ae7-p104">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="23ae7-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="23ae7-129">column</span><span class="sxs-lookup"><span data-stu-id="23ae7-129">column</span></span>|<span data-ttu-id="23ae7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="23ae7-130">Int32</span></span>|<span data-ttu-id="23ae7-p105">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="23ae7-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="23ae7-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23ae7-133">Request headers</span></span>
| <span data-ttu-id="23ae7-134">Nome</span><span class="sxs-lookup"><span data-stu-id="23ae7-134">Name</span></span>       | <span data-ttu-id="23ae7-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ae7-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23ae7-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="23ae7-136">Authorization</span></span>  | <span data-ttu-id="23ae7-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ae7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23ae7-139">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="23ae7-139">Workbook-Session-Id</span></span>  | <span data-ttu-id="23ae7-p107">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="23ae7-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ae7-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23ae7-142">Request body</span></span>
<span data-ttu-id="23ae7-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23ae7-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23ae7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ae7-144">Response</span></span>

<span data-ttu-id="23ae7-145">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23ae7-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ae7-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23ae7-146">Example</span></span>
<span data-ttu-id="23ae7-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="23ae7-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="23ae7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ae7-148">Request</span></span>
<span data-ttu-id="23ae7-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23ae7-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="23ae7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ae7-150">Response</span></span>
<span data-ttu-id="23ae7-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23ae7-151">Here is an example of the response.</span></span> <span data-ttu-id="23ae7-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23ae7-152">Note: The response object shown here might be shortened for readability.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


