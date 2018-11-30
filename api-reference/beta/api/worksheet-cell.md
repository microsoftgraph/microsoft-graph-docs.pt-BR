---
title: 'Worksheet: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.
ms.openlocfilehash: 5c85bf21e88b6b483abe1631c038e9239d3779d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034592"
---
# <a name="worksheet-cell"></a><span data-ttu-id="78661-104">Worksheet: Cell</span><span class="sxs-lookup"><span data-stu-id="78661-104">Worksheet: Cell</span></span>

> <span data-ttu-id="78661-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78661-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78661-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78661-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78661-p103">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.</span><span class="sxs-lookup"><span data-stu-id="78661-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="78661-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="78661-109">Permissions</span></span>
<span data-ttu-id="78661-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78661-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78661-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78661-112">Permission type</span></span>      | <span data-ttu-id="78661-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78661-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78661-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78661-114">Delegated (work or school account)</span></span> | <span data-ttu-id="78661-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78661-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="78661-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78661-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78661-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78661-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="78661-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78661-118">Application</span></span> | <span data-ttu-id="78661-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78661-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78661-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78661-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="78661-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="78661-121">Function parameters</span></span>
<span data-ttu-id="78661-122">Forneça o caminho da solicitação, os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="78661-122">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="78661-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="78661-123">Parameter</span></span>    | <span data-ttu-id="78661-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="78661-124">Type</span></span>   |<span data-ttu-id="78661-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="78661-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78661-126">row</span><span class="sxs-lookup"><span data-stu-id="78661-126">row</span></span>|<span data-ttu-id="78661-127">Int32</span><span class="sxs-lookup"><span data-stu-id="78661-127">Int32</span></span>|<span data-ttu-id="78661-p105">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="78661-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="78661-130">column</span><span class="sxs-lookup"><span data-stu-id="78661-130">column</span></span>|<span data-ttu-id="78661-131">Int32</span><span class="sxs-lookup"><span data-stu-id="78661-131">Int32</span></span>|<span data-ttu-id="78661-p106">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="78661-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="78661-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78661-134">Request headers</span></span>
| <span data-ttu-id="78661-135">Nome</span><span class="sxs-lookup"><span data-stu-id="78661-135">Name</span></span>       | <span data-ttu-id="78661-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="78661-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78661-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="78661-137">Authorization</span></span>  | <span data-ttu-id="78661-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78661-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78661-140">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="78661-140">Workbook-Session-Id</span></span>  | <span data-ttu-id="78661-p108">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="78661-p108">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78661-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78661-143">Request body</span></span>
<span data-ttu-id="78661-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78661-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78661-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="78661-145">Response</span></span>

<span data-ttu-id="78661-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78661-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78661-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78661-147">Example</span></span>
<span data-ttu-id="78661-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="78661-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="78661-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78661-149">Request</span></span>
<span data-ttu-id="78661-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78661-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="78661-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="78661-151">Response</span></span>
<span data-ttu-id="78661-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78661-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
