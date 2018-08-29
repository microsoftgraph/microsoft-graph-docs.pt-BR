# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="6c70a-101">Atualizar um formato de intervalo no Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c70a-101">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="6c70a-102">Os exemplos a seguir demonstram como atualizar as propriedades [RangeFormat](../api-reference/v1.0/resources/rangeformat.md), [RangeFill](../api-reference/v1.0/resources/rangefill.md) e [RangeFont](../api-reference/v1.0/resources/rangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="6c70a-102">The following examples demonstrate how to update properties of the [RangeFormat](../api-reference/v1.0/resources/rangeformat.md), [RangeFill](../api-reference/v1.0/resources/rangefill.md), and [RangeFont](../api-reference/v1.0/resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="6c70a-103">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="6c70a-103">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="6c70a-105">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-105">Request</span></span>
<span data-ttu-id="6c70a-106">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-106">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-107">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-107">Response</span></span>
<span data-ttu-id="6c70a-p101">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-111">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-111">Request</span></span>
<span data-ttu-id="6c70a-112">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-112">This request updates the font style, size, and color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-113">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-113">Response</span></span>
<span data-ttu-id="6c70a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-117">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-117">Request</span></span>
<span data-ttu-id="6c70a-118">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-118">This request updates the background color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-119">Response</span></span>
<span data-ttu-id="6c70a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="6c70a-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-123">Request</span></span>
<span data-ttu-id="6c70a-124">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-124">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-125">Response</span></span>
<span data-ttu-id="6c70a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-129">Request</span></span>
<span data-ttu-id="6c70a-130">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-130">This request updates the font style and size of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-131">Response</span></span>
<span data-ttu-id="6c70a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-135">Request</span></span>
<span data-ttu-id="6c70a-136">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-136">This request updates the background color of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-137">Response</span></span>
<span data-ttu-id="6c70a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-141">Request</span></span>
<span data-ttu-id="6c70a-142">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-142">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-143">Response</span></span>
<span data-ttu-id="6c70a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-147">Request</span></span>
<span data-ttu-id="6c70a-148">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-148">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="6c70a-149">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="6c70a-149">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-150">Response</span></span>
<span data-ttu-id="6c70a-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="6c70a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c70a-154">Request</span></span>
<span data-ttu-id="6c70a-155">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="6c70a-155">This request updates the background color of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="6c70a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c70a-156">Response</span></span>
<span data-ttu-id="6c70a-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c70a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="6c70a-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="6c70a-160">See also</span></span>
* [<span data-ttu-id="6c70a-161">Gerenciar sessões do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c70a-161">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="6c70a-162">Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c70a-162">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="6c70a-163">Usar funções de pasta de trabalho do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c70a-163">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="6c70a-164">Exibir uma imagem do gráfico do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c70a-164">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="6c70a-165">Usar a API REST do Excel</span><span class="sxs-lookup"><span data-stu-id="6c70a-165">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)
