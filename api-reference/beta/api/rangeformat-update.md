---
title: Atualizar rangeformat
description: Atualize as propriedades do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 169578d91ac115975f36c07c4405a810ad8c2da1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999227"
---
# <a name="update-rangeformat"></a><span data-ttu-id="5ebb9-103">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="5ebb9-103">Update rangeformat</span></span>

<span data-ttu-id="5ebb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ebb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ebb9-105">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ebb9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ebb9-106">Permissions</span></span>
<span data-ttu-id="5ebb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebb9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ebb9-109">Permission type</span></span>      | <span data-ttu-id="5ebb9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ebb9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ebb9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ebb9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ebb9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ebb9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ebb9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ebb9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ebb9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ebb9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ebb9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ebb9-115">Application</span></span> | <span data-ttu-id="5ebb9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ebb9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="5ebb9-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5ebb9-118">Optional request headers</span></span>
| <span data-ttu-id="5ebb9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5ebb9-119">Name</span></span>       | <span data-ttu-id="5ebb9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ebb9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5ebb9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ebb9-121">Authorization</span></span>  | <span data-ttu-id="5ebb9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ebb9-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ebb9-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ebb9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebb9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-127">Request body</span></span>
<span data-ttu-id="5ebb9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ebb9-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ebb9-131">Property</span></span>     | <span data-ttu-id="5ebb9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ebb9-132">Type</span></span>   |<span data-ttu-id="5ebb9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ebb9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ebb9-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="5ebb9-134">columnWidth</span></span>|<span data-ttu-id="5ebb9-135">duplo</span><span class="sxs-lookup"><span data-stu-id="5ebb9-135">double</span></span>|<span data-ttu-id="5ebb9-p105">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="5ebb9-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="5ebb9-138">horizontalAlignment</span></span>|<span data-ttu-id="5ebb9-139">string</span><span class="sxs-lookup"><span data-stu-id="5ebb9-139">string</span></span>|<span data-ttu-id="5ebb9-p106">Representa o alinhamento horizontal do objeto especificado. Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="5ebb9-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="5ebb9-142">rowHeight</span></span>|<span data-ttu-id="5ebb9-143">duplo</span><span class="sxs-lookup"><span data-stu-id="5ebb9-143">double</span></span>|<span data-ttu-id="5ebb9-p107">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="5ebb9-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="5ebb9-146">verticalAlignment</span></span>|<span data-ttu-id="5ebb9-147">string</span><span class="sxs-lookup"><span data-stu-id="5ebb9-147">string</span></span>|<span data-ttu-id="5ebb9-p108">Representa o alinhamento vertical do objeto especificado. Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify` e `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="5ebb9-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="5ebb9-150">wrapText</span></span>|<span data-ttu-id="5ebb9-151">booliano</span><span class="sxs-lookup"><span data-stu-id="5ebb9-151">boolean</span></span>|<span data-ttu-id="5ebb9-p109">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="5ebb9-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-154">Response</span></span>

<span data-ttu-id="5ebb9-155">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookRangeFormat](../resources/workbookrangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-155">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ebb9-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ebb9-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="5ebb9-157">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="5ebb9-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="5ebb9-158">Os exemplos a seguir demonstram como atualizar as propriedades das propriedades [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md)e [workbookRangeFont](../resources/workbookrangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-158">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="5ebb9-159">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="5ebb9-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-161">Request</span></span>
<span data-ttu-id="5ebb9-162">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-164">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-167">Response</span></span>
<span data-ttu-id="5ebb9-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-171">Request</span></span>
<span data-ttu-id="5ebb9-172">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-174">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-177">Response</span></span>
<span data-ttu-id="5ebb9-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-181">Request</span></span>
<span data-ttu-id="5ebb9-182">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-182">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-184">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-187">Response</span></span>
<span data-ttu-id="5ebb9-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="5ebb9-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-191">Request</span></span>
<span data-ttu-id="5ebb9-192">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-192">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-193">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-194">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-197">Response</span></span>
<span data-ttu-id="5ebb9-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-201">Request</span></span>
<span data-ttu-id="5ebb9-202">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-202">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-203">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-204">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-207">Response</span></span>
<span data-ttu-id="5ebb9-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-211">Request</span></span>
<span data-ttu-id="5ebb9-212">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-212">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-214">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-217">Response</span></span>
<span data-ttu-id="5ebb9-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-221">Request</span></span>
<span data-ttu-id="5ebb9-222">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-222">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-224">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-227">Response</span></span>
<span data-ttu-id="5ebb9-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-231">Request</span></span>
<span data-ttu-id="5ebb9-232">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-232">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="5ebb9-233">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-233">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ebb9-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-234">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-235">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-238">Response</span></span>
<span data-ttu-id="5ebb9-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5ebb9-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebb9-242">Request</span></span>
<span data-ttu-id="5ebb9-243">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-243">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5ebb9-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebb9-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebb9-245">C#</span><span class="sxs-lookup"><span data-stu-id="5ebb9-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebb9-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebb9-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebb9-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebb9-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebb9-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebb9-248">Response</span></span>
<span data-ttu-id="5ebb9-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebb9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


