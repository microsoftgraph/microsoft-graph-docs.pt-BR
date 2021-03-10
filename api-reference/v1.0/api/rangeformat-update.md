---
title: Atualizar rangeformat
description: Atualize as propriedades do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2eb4daf605bdebcf1885def6d2a66ced878ef81c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577783"
---
# <a name="update-rangeformat"></a><span data-ttu-id="32585-103">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="32585-103">Update rangeformat</span></span>

<span data-ttu-id="32585-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32585-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32585-105">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="32585-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="32585-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="32585-106">Permissions</span></span>
<span data-ttu-id="32585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32585-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32585-109">Permission type</span></span>      | <span data-ttu-id="32585-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32585-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32585-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32585-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32585-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32585-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32585-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32585-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32585-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32585-114">Not supported.</span></span>    |
|<span data-ttu-id="32585-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32585-115">Application</span></span> | <span data-ttu-id="32585-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32585-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32585-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="32585-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-118">Request headers</span></span>
| <span data-ttu-id="32585-119">Nome</span><span class="sxs-lookup"><span data-stu-id="32585-119">Name</span></span>       | <span data-ttu-id="32585-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="32585-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="32585-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="32585-121">Authorization</span></span>  | <span data-ttu-id="32585-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32585-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32585-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="32585-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="32585-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="32585-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32585-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-127">Request body</span></span>
<span data-ttu-id="32585-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="32585-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="32585-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32585-131">Property</span></span>     | <span data-ttu-id="32585-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="32585-132">Type</span></span>   |<span data-ttu-id="32585-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="32585-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32585-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="32585-134">columnWidth</span></span>|<span data-ttu-id="32585-135">duplo</span><span class="sxs-lookup"><span data-stu-id="32585-135">double</span></span>|<span data-ttu-id="32585-p105">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="32585-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="32585-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="32585-138">horizontalAlignment</span></span>|<span data-ttu-id="32585-139">string</span><span class="sxs-lookup"><span data-stu-id="32585-139">string</span></span>|<span data-ttu-id="32585-140">Representa o alinhamento horizontal do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="32585-140">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="32585-141">Os valores possíveis são: `General` , , , , , , , , `Left` `Center` `Right` `Fill` `Justify` `CenterAcrossSelection` `Distributed` .</span><span class="sxs-lookup"><span data-stu-id="32585-141">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="32585-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="32585-142">rowHeight</span></span>|<span data-ttu-id="32585-143">duplo</span><span class="sxs-lookup"><span data-stu-id="32585-143">double</span></span>|<span data-ttu-id="32585-p107">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="32585-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="32585-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="32585-146">verticalAlignment</span></span>|<span data-ttu-id="32585-147">string</span><span class="sxs-lookup"><span data-stu-id="32585-147">string</span></span>|<span data-ttu-id="32585-148">Representa o alinhamento vertical do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="32585-148">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="32585-149">Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="32585-149">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="32585-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="32585-150">wrapText</span></span>|<span data-ttu-id="32585-151">booliano</span><span class="sxs-lookup"><span data-stu-id="32585-151">boolean</span></span>|<span data-ttu-id="32585-p109">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="32585-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="32585-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-154">Response</span></span>

<span data-ttu-id="32585-155">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookRangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32585-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32585-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32585-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="32585-157">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="32585-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="32585-158">Os exemplos a seguir demonstram como atualizar propriedades das propriedades [WorkbookRangeFormat,](../resources/rangeformat.md) [WorkbookRangeFill](../resources/rangefill.md)e [WorkbookRangeFont](../resources/rangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="32585-158">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="32585-159">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="32585-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="32585-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-161">Request</span></span>
<span data-ttu-id="32585-162">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="32585-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-164">C#</span><span class="sxs-lookup"><span data-stu-id="32585-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-167">Java</span><span class="sxs-lookup"><span data-stu-id="32585-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-168">Response</span></span>
<span data-ttu-id="32585-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-172">Request</span></span>
<span data-ttu-id="32585-173">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="32585-173">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-175">C#</span><span class="sxs-lookup"><span data-stu-id="32585-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-178">Java</span><span class="sxs-lookup"><span data-stu-id="32585-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-179">Response</span></span>
<span data-ttu-id="32585-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-183">Request</span></span>
<span data-ttu-id="32585-184">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="32585-184">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-186">C#</span><span class="sxs-lookup"><span data-stu-id="32585-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-189">Java</span><span class="sxs-lookup"><span data-stu-id="32585-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-190">Response</span></span>
<span data-ttu-id="32585-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="32585-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-194">Request</span></span>
<span data-ttu-id="32585-195">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="32585-195">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-196">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-197">C#</span><span class="sxs-lookup"><span data-stu-id="32585-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-200">Java</span><span class="sxs-lookup"><span data-stu-id="32585-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-201">Response</span></span>
<span data-ttu-id="32585-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-205">Request</span></span>
<span data-ttu-id="32585-206">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="32585-206">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-207">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-208">C#</span><span class="sxs-lookup"><span data-stu-id="32585-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-211">Java</span><span class="sxs-lookup"><span data-stu-id="32585-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-212">Response</span></span>
<span data-ttu-id="32585-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-216">Request</span></span>
<span data-ttu-id="32585-217">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="32585-217">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-218">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-219">C#</span><span class="sxs-lookup"><span data-stu-id="32585-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-222">Java</span><span class="sxs-lookup"><span data-stu-id="32585-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-223">Response</span></span>
<span data-ttu-id="32585-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-227">Request</span></span>
<span data-ttu-id="32585-228">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="32585-228">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-229">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-230">C#</span><span class="sxs-lookup"><span data-stu-id="32585-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-233">Java</span><span class="sxs-lookup"><span data-stu-id="32585-233">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-234">Response</span></span>
<span data-ttu-id="32585-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-238">Request</span></span>
<span data-ttu-id="32585-239">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="32585-239">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="32585-240">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="32585-240">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="32585-241">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-241">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-242">C#</span><span class="sxs-lookup"><span data-stu-id="32585-242">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-243">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-243">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-244">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-244">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-245">Java</span><span class="sxs-lookup"><span data-stu-id="32585-245">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-246">Response</span></span>
<span data-ttu-id="32585-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="32585-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32585-250">Request</span></span>
<span data-ttu-id="32585-251">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="32585-251">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="32585-252">HTTP</span><span class="sxs-lookup"><span data-stu-id="32585-252">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32585-253">C#</span><span class="sxs-lookup"><span data-stu-id="32585-253">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32585-254">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32585-254">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32585-255">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32585-255">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32585-256">Java</span><span class="sxs-lookup"><span data-stu-id="32585-256">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32585-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="32585-257">Response</span></span>
<span data-ttu-id="32585-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32585-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->

