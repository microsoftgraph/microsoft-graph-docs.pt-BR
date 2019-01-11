---
title: 'Range: Cell'
description: Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.
localization_priority: Normal
ms.openlocfilehash: 2806fdcdc6072067a4fb4012fb9dc908aa3c15f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877011"
---
# <a name="range-cell"></a><span data-ttu-id="91f1d-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="91f1d-105">Range: Cell</span></span>

> <span data-ttu-id="91f1d-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91f1d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91f1d-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91f1d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91f1d-p103">Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.</span><span class="sxs-lookup"><span data-stu-id="91f1d-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="91f1d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="91f1d-111">Permissions</span></span>
<span data-ttu-id="91f1d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91f1d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f1d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91f1d-114">Permission type</span></span>      | <span data-ttu-id="91f1d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91f1d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91f1d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91f1d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="91f1d-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91f1d-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91f1d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91f1d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91f1d-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91f1d-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91f1d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91f1d-120">Application</span></span> | <span data-ttu-id="91f1d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91f1d-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91f1d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91f1d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="91f1d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91f1d-123">Request headers</span></span>
| <span data-ttu-id="91f1d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="91f1d-124">Name</span></span>       | <span data-ttu-id="91f1d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f1d-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91f1d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="91f1d-126">Authorization</span></span>  | <span data-ttu-id="91f1d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91f1d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91f1d-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="91f1d-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="91f1d-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="91f1d-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f1d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91f1d-132">Request body</span></span>
<span data-ttu-id="91f1d-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91f1d-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="91f1d-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="91f1d-134">Parameter</span></span>    | <span data-ttu-id="91f1d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="91f1d-135">Type</span></span>   |<span data-ttu-id="91f1d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f1d-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91f1d-137">row</span><span class="sxs-lookup"><span data-stu-id="91f1d-137">row</span></span>|<span data-ttu-id="91f1d-138">number</span><span class="sxs-lookup"><span data-stu-id="91f1d-138">number</span></span>|<span data-ttu-id="91f1d-p107">O número da linha da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="91f1d-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="91f1d-141">column</span><span class="sxs-lookup"><span data-stu-id="91f1d-141">column</span></span>|<span data-ttu-id="91f1d-142">number</span><span class="sxs-lookup"><span data-stu-id="91f1d-142">number</span></span>|<span data-ttu-id="91f1d-p108">O número da coluna da célula a ser recuperada. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="91f1d-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="91f1d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f1d-145">Response</span></span>

<span data-ttu-id="91f1d-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91f1d-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f1d-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91f1d-147">Example</span></span>
<span data-ttu-id="91f1d-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="91f1d-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91f1d-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91f1d-149">Request</span></span>
<span data-ttu-id="91f1d-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91f1d-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="91f1d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f1d-151">Response</span></span>
<span data-ttu-id="91f1d-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91f1d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
