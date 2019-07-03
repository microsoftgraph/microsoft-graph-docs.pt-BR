---
title: Atualizar um formato de intervalo no Excel com o Microsoft Graph
description: Os exemplos a seguir demonstram como atualizar as propriedades RangeFormat, RangeFill e RangeFont de um intervalo especificado.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 9874a24848126cfd065158a318699606fc02e352
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460802"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="693cb-103">Atualizar um formato de intervalo no Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="693cb-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="693cb-104">Os exemplos a seguir demonstram como atualizar as propriedades [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0) e [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) de um intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="693cb-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="693cb-105">O resultado desse conjunto de solicitações é uma tabela com três células formatadas como as três células principais na imagem abaixo.</span><span class="sxs-lookup"><span data-stu-id="693cb-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Tabela de gráfico do Excel com três células cujas propriedades formatação, preenchimento e fonte foram atualizadas.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="693cb-107">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-107">Request</span></span>
<span data-ttu-id="693cb-108">Esta solicitação atualiza o alinhamento vertical, a altura da linha e a altura da coluna da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-109">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-109">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-110">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-110">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-111">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-111">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-112">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-112">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-113">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-113">Response</span></span>
<span data-ttu-id="693cb-p101">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-117">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-117">Request</span></span>
<span data-ttu-id="693cb-118">Esta solicitação atualiza o estilo, o tamanho e a cor da fonte da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-118">This request updates the font style, size, and color of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-119">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-120">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-122">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-123">Response</span></span>
<span data-ttu-id="693cb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-127">Request</span></span>
<span data-ttu-id="693cb-128">Esta solicitação atualiza a cor da tela de fundo da primeira célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-128">This request updates the background color of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-130">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-133">Response</span></span>
<span data-ttu-id="693cb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="693cb-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-137">Request</span></span>
<span data-ttu-id="693cb-138">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-138">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-140">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-143">Response</span></span>
<span data-ttu-id="693cb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-147">Request</span></span>
<span data-ttu-id="693cb-148">Esta solicitação atualiza o estilo e o tamanho da fonte da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-148">This request updates the font style and size of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-150">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-153">Response</span></span>
<span data-ttu-id="693cb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-157">Request</span></span>
<span data-ttu-id="693cb-158">Esta solicitação atualiza a cor da tela de fundo da segunda célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-158">This request updates the background color of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-160">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-163">Response</span></span>
<span data-ttu-id="693cb-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-167">Request</span></span>
<span data-ttu-id="693cb-168">Esta solicitação atualiza o alinhamento vertical, o alinhamento horizontal, a altura da linha e a altura da coluna da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-168">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-169">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-170">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-173">Response</span></span>
<span data-ttu-id="693cb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-177">Request</span></span>
<span data-ttu-id="693cb-178">Esta solicitação atualiza o estilo da fonte, o tamanho e a cor da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-178">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="693cb-179">A propriedade underline tem **Single** ou **Double** como valores.</span><span class="sxs-lookup"><span data-stu-id="693cb-179">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-180">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-181">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-184">Response</span></span>
<span data-ttu-id="693cb-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="693cb-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="693cb-188">Request</span></span>
<span data-ttu-id="693cb-189">Esta solicitação atualiza a cor da tela de fundo da terceira célula.</span><span class="sxs-lookup"><span data-stu-id="693cb-189">This request updates the background color of the third cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="693cb-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="693cb-190">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="693cb-191">C#</span><span class="sxs-lookup"><span data-stu-id="693cb-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="693cb-192">Javascript</span><span class="sxs-lookup"><span data-stu-id="693cb-192">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="693cb-193">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="693cb-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="693cb-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="693cb-194">Response</span></span>
<span data-ttu-id="693cb-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="693cb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="693cb-198">Confira também</span><span class="sxs-lookup"><span data-stu-id="693cb-198">See also</span></span>
* [<span data-ttu-id="693cb-199">Gerenciar sessões do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="693cb-199">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="693cb-200">Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="693cb-200">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="693cb-201">Usar funções de pasta de trabalho do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="693cb-201">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="693cb-202">Exibir uma imagem do gráfico do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="693cb-202">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="693cb-203">Usar a API REST do Excel</span><span class="sxs-lookup"><span data-stu-id="693cb-203">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update a range format in Excel with Microsoft Graph",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
