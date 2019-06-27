---
title: Atualizar rangeformat
description: Atualize as propriedades do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 31023749e119722c0f393fe8def05edf2a3e23a4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263619"
---
# <a name="update-rangeformat"></a><span data-ttu-id="c72af-103">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="c72af-103">Update rangeformat</span></span>

<span data-ttu-id="c72af-104">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="c72af-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c72af-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c72af-105">Permissions</span></span>
<span data-ttu-id="c72af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c72af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c72af-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c72af-108">Permission type</span></span>      | <span data-ttu-id="c72af-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c72af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c72af-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c72af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c72af-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c72af-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c72af-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c72af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c72af-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c72af-113">Not supported.</span></span>    |
|<span data-ttu-id="c72af-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c72af-114">Application</span></span> | <span data-ttu-id="c72af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c72af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c72af-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c72af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="c72af-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-117">Request headers</span></span>
| <span data-ttu-id="c72af-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c72af-118">Name</span></span>       | <span data-ttu-id="c72af-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c72af-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c72af-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c72af-120">Authorization</span></span>  | <span data-ttu-id="c72af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c72af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c72af-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c72af-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c72af-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c72af-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c72af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-126">Request body</span></span>
<span data-ttu-id="c72af-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c72af-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c72af-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c72af-130">Property</span></span>     | <span data-ttu-id="c72af-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c72af-131">Type</span></span>   |<span data-ttu-id="c72af-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c72af-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c72af-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="c72af-133">columnWidth</span></span>|<span data-ttu-id="c72af-134">double</span><span class="sxs-lookup"><span data-stu-id="c72af-134">double</span></span>|<span data-ttu-id="c72af-p105">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="c72af-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="c72af-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="c72af-137">horizontalAlignment</span></span>|<span data-ttu-id="c72af-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c72af-138">string</span></span>|<span data-ttu-id="c72af-139">Representa o alinhamento horizontal do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="c72af-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="c72af-140">Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="c72af-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="c72af-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="c72af-141">rowHeight</span></span>|<span data-ttu-id="c72af-142">duplo</span><span class="sxs-lookup"><span data-stu-id="c72af-142">double</span></span>|<span data-ttu-id="c72af-p107">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="c72af-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="c72af-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="c72af-145">verticalAlignment</span></span>|<span data-ttu-id="c72af-146">string</span><span class="sxs-lookup"><span data-stu-id="c72af-146">string</span></span>|<span data-ttu-id="c72af-147">Representa o alinhamento vertical do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="c72af-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="c72af-148">Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="c72af-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="c72af-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="c72af-149">wrapText</span></span>|<span data-ttu-id="c72af-150">booliano</span><span class="sxs-lookup"><span data-stu-id="c72af-150">boolean</span></span>|<span data-ttu-id="c72af-p109">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="c72af-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="c72af-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-153">Response</span></span>

<span data-ttu-id="c72af-154">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookRangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c72af-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c72af-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c72af-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="c72af-156">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="c72af-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="c72af-157">Os exemplos a seguir demonstram como atualizar as propriedades das propriedades [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md)e [WorkbookRangeFont](../resources/rangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="c72af-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="c72af-158">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="c72af-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="c72af-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-160">Request</span></span>
<span data-ttu-id="c72af-161">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="c72af-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-162">Response</span></span>
<span data-ttu-id="c72af-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-166">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-167">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-169">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-170">Request</span></span>
<span data-ttu-id="c72af-171">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-171">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="c72af-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-172">Response</span></span>
<span data-ttu-id="c72af-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-176">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-177">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-179">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-180">Request</span></span>
<span data-ttu-id="c72af-181">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-181">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="c72af-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-182">Response</span></span>
<span data-ttu-id="c72af-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-186">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-187">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-189">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="c72af-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-190">Request</span></span>
<span data-ttu-id="c72af-191">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-191">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="c72af-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-192">Response</span></span>
<span data-ttu-id="c72af-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-196">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-196">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-197">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-197">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-198">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-198">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-199">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-199">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-200">Request</span></span>
<span data-ttu-id="c72af-201">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-201">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="c72af-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-202">Response</span></span>
<span data-ttu-id="c72af-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-206">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-207">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-209">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-209">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-210">Request</span></span>
<span data-ttu-id="c72af-211">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-211">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="c72af-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-212">Response</span></span>
<span data-ttu-id="c72af-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-216">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-216">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-217">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-217">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-218">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-218">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-219">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-219">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-220">Request</span></span>
<span data-ttu-id="c72af-221">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-221">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="c72af-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-222">Response</span></span>
<span data-ttu-id="c72af-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-226">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-226">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-227">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-227">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-229">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-229">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-230">Request</span></span>
<span data-ttu-id="c72af-231">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-231">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="c72af-232">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="c72af-232">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="c72af-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-233">Response</span></span>
<span data-ttu-id="c72af-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-237">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-237">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-238">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-238">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-239">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-239">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-240">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-240">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="c72af-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c72af-241">Request</span></span>
<span data-ttu-id="c72af-242">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="c72af-242">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="c72af-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="c72af-243">Response</span></span>
<span data-ttu-id="c72af-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c72af-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c72af-247">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c72af-247">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c72af-248">C#</span><span class="sxs-lookup"><span data-stu-id="c72af-248">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c72af-249">Javascript</span><span class="sxs-lookup"><span data-stu-id="c72af-249">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c72af-250">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c72af-250">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->
