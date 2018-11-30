---
title: 'Worksheet: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.
ms.openlocfilehash: 5e9134fe9ba685a5770cf0671ce06e740a886891
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006064"
---
# <a name="worksheet-cell"></a><span data-ttu-id="26e78-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="26e78-104">Worksheet: Cell</span></span>

<span data-ttu-id="26e78-p102">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="26e78-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="26e78-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="26e78-107">Permissions</span></span>
<span data-ttu-id="26e78-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e78-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26e78-110">Permission type</span></span>      | <span data-ttu-id="26e78-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26e78-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26e78-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26e78-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26e78-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e78-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26e78-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26e78-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26e78-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26e78-115">Not supported.</span></span>    |
|<span data-ttu-id="26e78-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26e78-116">Application</span></span> | <span data-ttu-id="26e78-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26e78-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26e78-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26e78-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="26e78-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="26e78-119">Function parameters</span></span>
<span data-ttu-id="26e78-120">Forneça o caminho da solicitação, os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="26e78-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="26e78-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="26e78-121">Parameter</span></span>    | <span data-ttu-id="26e78-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="26e78-122">Type</span></span>   |<span data-ttu-id="26e78-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e78-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26e78-124">row</span><span class="sxs-lookup"><span data-stu-id="26e78-124">row</span></span>|<span data-ttu-id="26e78-125">Int32</span><span class="sxs-lookup"><span data-stu-id="26e78-125">Int32</span></span>|<span data-ttu-id="26e78-p104">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="26e78-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="26e78-128">column</span><span class="sxs-lookup"><span data-stu-id="26e78-128">column</span></span>|<span data-ttu-id="26e78-129">Int32</span><span class="sxs-lookup"><span data-stu-id="26e78-129">Int32</span></span>|<span data-ttu-id="26e78-p105">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="26e78-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="26e78-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26e78-132">Request headers</span></span>
| <span data-ttu-id="26e78-133">Nome</span><span class="sxs-lookup"><span data-stu-id="26e78-133">Name</span></span>       | <span data-ttu-id="26e78-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e78-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26e78-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="26e78-135">Authorization</span></span>  | <span data-ttu-id="26e78-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26e78-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26e78-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="26e78-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="26e78-p107">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="26e78-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e78-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26e78-141">Request body</span></span>
<span data-ttu-id="26e78-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26e78-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26e78-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="26e78-143">Response</span></span>

<span data-ttu-id="26e78-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26e78-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e78-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26e78-145">Example</span></span>
<span data-ttu-id="26e78-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="26e78-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="26e78-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26e78-147">Request</span></span>
<span data-ttu-id="26e78-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26e78-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="26e78-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="26e78-149">Response</span></span>
<span data-ttu-id="26e78-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26e78-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
