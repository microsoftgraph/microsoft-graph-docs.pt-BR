---
title: Atualizar rangeformat
description: Atualize as propriedades do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 70b3d598923583b297028a6f9adf31abf9288452
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050385"
---
# <a name="update-rangeformat"></a><span data-ttu-id="c54f6-103">Atualizar rangeformat</span><span class="sxs-lookup"><span data-stu-id="c54f6-103">Update rangeformat</span></span>

<span data-ttu-id="c54f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c54f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c54f6-105">Atualize as propriedades do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="c54f6-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c54f6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c54f6-106">Permissions</span></span>
<span data-ttu-id="c54f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54f6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c54f6-109">Permission type</span></span>      | <span data-ttu-id="c54f6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c54f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c54f6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c54f6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c54f6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c54f6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c54f6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c54f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c54f6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c54f6-114">Not supported.</span></span>    |
|<span data-ttu-id="c54f6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c54f6-115">Application</span></span> | <span data-ttu-id="c54f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c54f6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c54f6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="c54f6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-118">Request headers</span></span>
| <span data-ttu-id="c54f6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c54f6-119">Name</span></span>       | <span data-ttu-id="c54f6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54f6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c54f6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c54f6-121">Authorization</span></span>  | <span data-ttu-id="c54f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c54f6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c54f6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c54f6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c54f6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c54f6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c54f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-127">Request body</span></span>
<span data-ttu-id="c54f6-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c54f6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c54f6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c54f6-131">Property</span></span>     | <span data-ttu-id="c54f6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c54f6-132">Type</span></span>   |<span data-ttu-id="c54f6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54f6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c54f6-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="c54f6-134">columnWidth</span></span>|<span data-ttu-id="c54f6-135">duplo</span><span class="sxs-lookup"><span data-stu-id="c54f6-135">double</span></span>|<span data-ttu-id="c54f6-p105">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="c54f6-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="c54f6-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="c54f6-138">horizontalAlignment</span></span>|<span data-ttu-id="c54f6-139">string</span><span class="sxs-lookup"><span data-stu-id="c54f6-139">string</span></span>|<span data-ttu-id="c54f6-140">Representa o alinhamento horizontal do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="c54f6-140">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="c54f6-141">Os valores possíveis são: `General` , , , , , , , , `Left` `Center` `Right` `Fill` `Justify` `CenterAcrossSelection` `Distributed` .</span><span class="sxs-lookup"><span data-stu-id="c54f6-141">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="c54f6-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="c54f6-142">rowHeight</span></span>|<span data-ttu-id="c54f6-143">duplo</span><span class="sxs-lookup"><span data-stu-id="c54f6-143">double</span></span>|<span data-ttu-id="c54f6-p107">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="c54f6-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="c54f6-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="c54f6-146">verticalAlignment</span></span>|<span data-ttu-id="c54f6-147">string</span><span class="sxs-lookup"><span data-stu-id="c54f6-147">string</span></span>|<span data-ttu-id="c54f6-148">Representa o alinhamento vertical do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="c54f6-148">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="c54f6-149">Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="c54f6-149">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="c54f6-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="c54f6-150">wrapText</span></span>|<span data-ttu-id="c54f6-151">booliano</span><span class="sxs-lookup"><span data-stu-id="c54f6-151">boolean</span></span>|<span data-ttu-id="c54f6-p109">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="c54f6-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="c54f6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-154">Response</span></span>

<span data-ttu-id="c54f6-155">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookRangeFormat](../resources/rangeformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c54f6-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c54f6-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="c54f6-157">Atualizar as propriedades de fonte, formatação e preenchimento em três células de tabela</span><span class="sxs-lookup"><span data-stu-id="c54f6-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="c54f6-158">Os exemplos a seguir demonstram como atualizar propriedades das propriedades [WorkbookRangeFormat,](../resources/rangeformat.md) [WorkbookRangeFill](../resources/rangefill.md)e [WorkbookRangeFont](../resources/rangefont.md) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="c54f6-158">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="c54f6-159">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="c54f6-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="c54f6-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-161">Request</span></span>
<span data-ttu-id="c54f6-162">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-164">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-167">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-168">Response</span></span>
<span data-ttu-id="c54f6-169">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-169">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-170">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-170">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-171">Request</span></span>
<span data-ttu-id="c54f6-172">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-174">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-177">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-178">Response</span></span>
<span data-ttu-id="c54f6-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-179">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-180">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-180">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-181">Request</span></span>
<span data-ttu-id="c54f6-182">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-182">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-184">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-187">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-188">Response</span></span>
<span data-ttu-id="c54f6-189">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-189">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-190">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-190">Note: The response object shown here might be shortened for readability.</span></span>
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
##### <a name="request"></a><span data-ttu-id="c54f6-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-191">Request</span></span>
<span data-ttu-id="c54f6-192">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-192">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-193">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-194">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-197">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-198">Response</span></span>
<span data-ttu-id="c54f6-199">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-199">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-200">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-200">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-201">Request</span></span>
<span data-ttu-id="c54f6-202">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-202">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-203">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-204">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-207">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-208">Response</span></span>
<span data-ttu-id="c54f6-209">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-209">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-210">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-210">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-211">Request</span></span>
<span data-ttu-id="c54f6-212">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-212">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-214">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-217">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-218">Response</span></span>
<span data-ttu-id="c54f6-219">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-219">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-220">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-220">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-221">Request</span></span>
<span data-ttu-id="c54f6-222">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-222">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-224">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-227">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-228">Response</span></span>
<span data-ttu-id="c54f6-229">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-229">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-230">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-230">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-231">Request</span></span>
<span data-ttu-id="c54f6-232">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-232">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="c54f6-233">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="c54f6-233">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="c54f6-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-234">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-235">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-238">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-239">Response</span></span>
<span data-ttu-id="c54f6-240">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-240">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-241">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-241">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c54f6-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54f6-242">Request</span></span>
<span data-ttu-id="c54f6-243">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="c54f6-243">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c54f6-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54f6-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c54f6-245">C#</span><span class="sxs-lookup"><span data-stu-id="c54f6-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54f6-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54f6-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54f6-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54f6-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c54f6-248">Java</span><span class="sxs-lookup"><span data-stu-id="c54f6-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c54f6-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54f6-249">Response</span></span>
<span data-ttu-id="c54f6-250">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54f6-250">Here is an example of the response.</span></span> <span data-ttu-id="c54f6-251">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c54f6-251">Note: The response object shown here might be shortened for readability.</span></span>
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

