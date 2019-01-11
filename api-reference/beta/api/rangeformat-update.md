---
title: Atualizar rangeformat
description: Atualize as propriedades do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8d7df390628e1f8a4416042efe218e36c516a669
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873238"
---
# <a name="update-rangeformat"></a><span data-ttu-id="ec3a7-103">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="ec3a7-103">Update rangeformat</span></span>

> <span data-ttu-id="ec3a7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec3a7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec3a7-106">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-106">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec3a7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec3a7-107">Permissions</span></span>
<span data-ttu-id="ec3a7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec3a7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec3a7-110">Permission type</span></span>      | <span data-ttu-id="ec3a7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec3a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec3a7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec3a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec3a7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec3a7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec3a7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec3a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec3a7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec3a7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec3a7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec3a7-116">Application</span></span> | <span data-ttu-id="ec3a7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec3a7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec3a7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="ec3a7-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ec3a7-119">Optional request headers</span></span>
| <span data-ttu-id="ec3a7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ec3a7-120">Name</span></span>       | <span data-ttu-id="ec3a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec3a7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ec3a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec3a7-122">Authorization</span></span>  | <span data-ttu-id="ec3a7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec3a7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec3a7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec3a7-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec3a7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-128">Request body</span></span>
<span data-ttu-id="ec3a7-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ec3a7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec3a7-132">Property</span></span>     | <span data-ttu-id="ec3a7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec3a7-133">Type</span></span>   |<span data-ttu-id="ec3a7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec3a7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec3a7-135">columnWidth</span><span class="sxs-lookup"><span data-stu-id="ec3a7-135">columnWidth</span></span>|<span data-ttu-id="ec3a7-136">double</span><span class="sxs-lookup"><span data-stu-id="ec3a7-136">double</span></span>|<span data-ttu-id="ec3a7-p106">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p106">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="ec3a7-139">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="ec3a7-139">horizontalAlignment</span></span>|<span data-ttu-id="ec3a7-140">string</span><span class="sxs-lookup"><span data-stu-id="ec3a7-140">string</span></span>|<span data-ttu-id="ec3a7-p107">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p107">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="ec3a7-143">rowHeight</span><span class="sxs-lookup"><span data-stu-id="ec3a7-143">rowHeight</span></span>|<span data-ttu-id="ec3a7-144">double</span><span class="sxs-lookup"><span data-stu-id="ec3a7-144">double</span></span>|<span data-ttu-id="ec3a7-p108">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p108">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="ec3a7-147">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="ec3a7-147">verticalAlignment</span></span>|<span data-ttu-id="ec3a7-148">string</span><span class="sxs-lookup"><span data-stu-id="ec3a7-148">string</span></span>|<span data-ttu-id="ec3a7-p109">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p109">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="ec3a7-151">wrapText</span><span class="sxs-lookup"><span data-stu-id="ec3a7-151">wrapText</span></span>|<span data-ttu-id="ec3a7-152">booliano</span><span class="sxs-lookup"><span data-stu-id="ec3a7-152">boolean</span></span>|<span data-ttu-id="ec3a7-p110">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p110">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="ec3a7-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-155">Response</span></span>

<span data-ttu-id="ec3a7-156">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-156">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec3a7-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec3a7-157">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="ec3a7-158">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="ec3a7-158">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="ec3a7-159">Os exemplos a seguir demonstram como atualizar as propriedades [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md) e [RangeFont](../resources/rangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-159">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="ec3a7-160">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-160">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="ec3a7-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-162">Request</span></span>
<span data-ttu-id="ec3a7-163">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-163">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-164">Response</span></span>
<span data-ttu-id="ec3a7-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-168">Request</span></span>
<span data-ttu-id="ec3a7-169">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-169">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-170">Response</span></span>
<span data-ttu-id="ec3a7-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-174">Request</span></span>
<span data-ttu-id="ec3a7-175">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-175">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-176">Response</span></span>
<span data-ttu-id="ec3a7-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="ec3a7-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-180">Request</span></span>
<span data-ttu-id="ec3a7-181">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-181">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-182">Response</span></span>
<span data-ttu-id="ec3a7-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-186">Request</span></span>
<span data-ttu-id="ec3a7-187">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-187">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-188">Response</span></span>
<span data-ttu-id="ec3a7-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-192">Request</span></span>
<span data-ttu-id="ec3a7-193">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-193">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-194">Response</span></span>
<span data-ttu-id="ec3a7-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-198">Request</span></span>
<span data-ttu-id="ec3a7-199">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-199">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-200">Response</span></span>
<span data-ttu-id="ec3a7-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-204">Request</span></span>
<span data-ttu-id="ec3a7-205">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-205">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="ec3a7-206">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-206">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="ec3a7-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-207">Response</span></span>
<span data-ttu-id="ec3a7-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="ec3a7-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec3a7-211">Request</span></span>
<span data-ttu-id="ec3a7-212">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-212">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="ec3a7-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec3a7-213">Response</span></span>
<span data-ttu-id="ec3a7-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec3a7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
