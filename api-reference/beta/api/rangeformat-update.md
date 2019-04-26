---
title: Atualizar rangeformat
description: Atualize as propriedades do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c0d285a82b34ce06d8a10c784a124cc03519e1c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331793"
---
# <a name="update-rangeformat"></a><span data-ttu-id="f5f62-103">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="f5f62-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f62-104">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="f5f62-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5f62-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5f62-105">Permissions</span></span>
<span data-ttu-id="f5f62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5f62-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5f62-108">Permission type</span></span>      | <span data-ttu-id="f5f62-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5f62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5f62-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5f62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f5f62-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5f62-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5f62-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5f62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5f62-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5f62-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5f62-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5f62-114">Application</span></span> | <span data-ttu-id="f5f62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f62-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5f62-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="f5f62-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f5f62-117">Optional request headers</span></span>
| <span data-ttu-id="f5f62-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f5f62-118">Name</span></span>       | <span data-ttu-id="f5f62-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f62-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f5f62-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5f62-120">Authorization</span></span>  | <span data-ttu-id="f5f62-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5f62-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f5f62-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5f62-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5f62-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-126">Request body</span></span>
<span data-ttu-id="f5f62-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5f62-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5f62-130">Property</span></span>     | <span data-ttu-id="f5f62-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5f62-131">Type</span></span>   |<span data-ttu-id="f5f62-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f62-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5f62-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="f5f62-133">columnWidth</span></span>|<span data-ttu-id="f5f62-134">double</span><span class="sxs-lookup"><span data-stu-id="f5f62-134">double</span></span>|<span data-ttu-id="f5f62-p105">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="f5f62-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="f5f62-137">horizontalAlignment</span></span>|<span data-ttu-id="f5f62-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f62-138">string</span></span>|<span data-ttu-id="f5f62-p106">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="f5f62-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="f5f62-141">rowHeight</span></span>|<span data-ttu-id="f5f62-142">duplo</span><span class="sxs-lookup"><span data-stu-id="f5f62-142">double</span></span>|<span data-ttu-id="f5f62-p107">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="f5f62-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="f5f62-145">verticalAlignment</span></span>|<span data-ttu-id="f5f62-146">string</span><span class="sxs-lookup"><span data-stu-id="f5f62-146">string</span></span>|<span data-ttu-id="f5f62-p108">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="f5f62-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="f5f62-149">wrapText</span></span>|<span data-ttu-id="f5f62-150">booliano</span><span class="sxs-lookup"><span data-stu-id="f5f62-150">boolean</span></span>|<span data-ttu-id="f5f62-p109">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="f5f62-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-153">Response</span></span>

<span data-ttu-id="f5f62-154">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookRangeFormat](../resources/workbookrangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f62-154">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5f62-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5f62-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="f5f62-156">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="f5f62-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="f5f62-157">Os exemplos a seguir demonstram como atualizar as propriedades das propriedades [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md)e [workbookRangeFont](../resources/workbookrangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="f5f62-157">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="f5f62-158">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="f5f62-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="f5f62-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-160">Request</span></span>
<span data-ttu-id="f5f62-161">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-162">Response</span></span>
<span data-ttu-id="f5f62-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "General",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-166">Request</span></span>
<span data-ttu-id="f5f62-167">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-167">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-168">Response</span></span>
<span data-ttu-id="f5f62-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": true,
    "color": "#4B180E",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-172">Request</span></span>
<span data-ttu-id="f5f62-173">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-173">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-174">Response</span></span>
<span data-ttu-id="f5f62-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="f5f62-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-178">Request</span></span>
<span data-ttu-id="f5f62-179">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-180">Response</span></span>
<span data-ttu-id="f5f62-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Center",
    "rowHeight": 49,
    "verticalAlignment": "Center",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-184">Request</span></span>
<span data-ttu-id="f5f62-185">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-185">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-186">Response</span></span>
<span data-ttu-id="f5f62-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#000000",
    "italic": true,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-190">Request</span></span>
<span data-ttu-id="f5f62-191">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-191">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-192">Response</span></span>
<span data-ttu-id="f5f62-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-196">Request</span></span>
<span data-ttu-id="f5f62-197">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-198">Response</span></span>
<span data-ttu-id="f5f62-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Right",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-202">Request</span></span>
<span data-ttu-id="f5f62-203">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="f5f62-204">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="f5f62-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-205">Response</span></span>
<span data-ttu-id="f5f62-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#FFFFFF",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "Single"
}
```

##### <a name="request"></a><span data-ttu-id="f5f62-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f62-209">Request</span></span>
<span data-ttu-id="f5f62-210">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="f5f62-210">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="f5f62-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f62-211">Response</span></span>
<span data-ttu-id="f5f62-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f62-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:\r\n       Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ]
}
-->
