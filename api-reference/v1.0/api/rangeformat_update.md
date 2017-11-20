# <a name="update-rangeformat"></a><span data-ttu-id="170b3-101">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="170b3-101">Update rangeformat</span></span>

<span data-ttu-id="170b3-102">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="170b3-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="170b3-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="170b3-103">Permissions</span></span>
<span data-ttu-id="170b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="170b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="170b3-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="170b3-106">Permission type</span></span>      | <span data-ttu-id="170b3-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="170b3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170b3-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="170b3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="170b3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170b3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="170b3-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="170b3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170b3-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="170b3-111">Not supported.</span></span>    |
|<span data-ttu-id="170b3-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="170b3-112">Application</span></span> | <span data-ttu-id="170b3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="170b3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="170b3-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="170b3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="170b3-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="170b3-115">Optional request headers</span></span>
| <span data-ttu-id="170b3-116">Nome</span><span class="sxs-lookup"><span data-stu-id="170b3-116">Name</span></span>       | <span data-ttu-id="170b3-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="170b3-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="170b3-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="170b3-118">Authorization</span></span>  | <span data-ttu-id="170b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="170b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="170b3-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-121">Request body</span></span>
<span data-ttu-id="170b3-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="170b3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="170b3-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="170b3-125">Property</span></span>     | <span data-ttu-id="170b3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="170b3-126">Type</span></span>   |<span data-ttu-id="170b3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="170b3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="170b3-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="170b3-128">columnWidth</span></span>|<span data-ttu-id="170b3-129">double</span><span class="sxs-lookup"><span data-stu-id="170b3-129">double</span></span>|<span data-ttu-id="170b3-p104">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="170b3-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="170b3-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="170b3-132">horizontalAlignment</span></span>|<span data-ttu-id="170b3-133">string</span><span class="sxs-lookup"><span data-stu-id="170b3-133">string</span></span>|<span data-ttu-id="170b3-p105">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="170b3-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="170b3-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="170b3-136">rowHeight</span></span>|<span data-ttu-id="170b3-137">double</span><span class="sxs-lookup"><span data-stu-id="170b3-137">double</span></span>|<span data-ttu-id="170b3-p106">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="170b3-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="170b3-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="170b3-140">verticalAlignment</span></span>|<span data-ttu-id="170b3-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="170b3-141">string</span></span>|<span data-ttu-id="170b3-p107">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="170b3-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="170b3-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="170b3-144">wrapText</span></span>|<span data-ttu-id="170b3-145">booliano</span><span class="sxs-lookup"><span data-stu-id="170b3-145">boolean</span></span>|<span data-ttu-id="170b3-p108">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="170b3-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="170b3-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-148">Response</span></span>

<span data-ttu-id="170b3-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="170b3-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="170b3-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="170b3-150">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="170b3-151">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="170b3-151">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="170b3-152">Os exemplos a seguir demonstram como atualizar as propriedades [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md) e [RangeFont](../resources/rangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="170b3-152">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="170b3-153">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="170b3-153">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="170b3-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-155">Request</span></span>
<span data-ttu-id="170b3-156">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-156">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="170b3-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-157">Response</span></span>
<span data-ttu-id="170b3-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="170b3-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-161">Request</span></span>
<span data-ttu-id="170b3-162">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-162">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="170b3-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-163">Response</span></span>
<span data-ttu-id="170b3-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="170b3-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-167">Request</span></span>
<span data-ttu-id="170b3-168">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-168">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="170b3-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-169">Response</span></span>
<span data-ttu-id="170b3-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="170b3-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-173">Request</span></span>
<span data-ttu-id="170b3-174">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-174">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="170b3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-175">Response</span></span>
<span data-ttu-id="170b3-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="170b3-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-179">Request</span></span>
<span data-ttu-id="170b3-180">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-180">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="170b3-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-181">Response</span></span>
<span data-ttu-id="170b3-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="170b3-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-185">Request</span></span>
<span data-ttu-id="170b3-186">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-186">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="170b3-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-187">Response</span></span>
<span data-ttu-id="170b3-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="170b3-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-191">Request</span></span>
<span data-ttu-id="170b3-192">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-192">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="170b3-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-193">Response</span></span>
<span data-ttu-id="170b3-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="170b3-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-197">Request</span></span>
<span data-ttu-id="170b3-198">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-198">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="170b3-199">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="170b3-199">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="170b3-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-200">Response</span></span>
<span data-ttu-id="170b3-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="170b3-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170b3-204">Request</span></span>
<span data-ttu-id="170b3-205">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="170b3-205">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="170b3-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="170b3-206">Response</span></span>
<span data-ttu-id="170b3-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="170b3-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->