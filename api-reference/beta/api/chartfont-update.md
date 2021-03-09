---
title: Atualizar a workbookChartFont
description: Atualize as propriedades do objeto workbookChartFont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b17313a909eddf7660bba1cca214fca54a9113a9
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574549"
---
# <a name="update-chartfont"></a><span data-ttu-id="d2fe7-103">Atualizar chartfont</span><span class="sxs-lookup"><span data-stu-id="d2fe7-103">Update chartfont</span></span>

<span data-ttu-id="d2fe7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2fe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2fe7-105">Atualiza as propriedades do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-105">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2fe7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2fe7-106">Permissions</span></span>
<span data-ttu-id="d2fe7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2fe7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2fe7-109">Permission type</span></span>      | <span data-ttu-id="d2fe7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2fe7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2fe7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2fe7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2fe7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2fe7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2fe7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2fe7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2fe7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2fe7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2fe7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2fe7-115">Application</span></span> | <span data-ttu-id="d2fe7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2fe7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2fe7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="d2fe7-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d2fe7-118">Optional request headers</span></span>
| <span data-ttu-id="d2fe7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d2fe7-119">Name</span></span>       | <span data-ttu-id="d2fe7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2fe7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d2fe7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2fe7-121">Authorization</span></span>  | <span data-ttu-id="d2fe7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2fe7-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2fe7-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2fe7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2fe7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2fe7-127">Request body</span></span>
<span data-ttu-id="d2fe7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d2fe7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2fe7-131">Property</span></span>     | <span data-ttu-id="d2fe7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2fe7-132">Type</span></span>   |<span data-ttu-id="d2fe7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2fe7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2fe7-134">bold</span><span class="sxs-lookup"><span data-stu-id="d2fe7-134">bold</span></span>|<span data-ttu-id="d2fe7-135">booliano</span><span class="sxs-lookup"><span data-stu-id="d2fe7-135">boolean</span></span>|<span data-ttu-id="d2fe7-136">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="d2fe7-137">color</span><span class="sxs-lookup"><span data-stu-id="d2fe7-137">color</span></span>|<span data-ttu-id="d2fe7-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2fe7-138">string</span></span>|<span data-ttu-id="d2fe7-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="d2fe7-142">italic</span><span class="sxs-lookup"><span data-stu-id="d2fe7-142">italic</span></span>|<span data-ttu-id="d2fe7-143">booliano</span><span class="sxs-lookup"><span data-stu-id="d2fe7-143">boolean</span></span>|<span data-ttu-id="d2fe7-144">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="d2fe7-145">nome</span><span class="sxs-lookup"><span data-stu-id="d2fe7-145">name</span></span>|<span data-ttu-id="d2fe7-146">string</span><span class="sxs-lookup"><span data-stu-id="d2fe7-146">string</span></span>|<span data-ttu-id="d2fe7-147">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="d2fe7-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="d2fe7-148">size</span><span class="sxs-lookup"><span data-stu-id="d2fe7-148">size</span></span>|<span data-ttu-id="d2fe7-149">Double</span><span class="sxs-lookup"><span data-stu-id="d2fe7-149">double</span></span>|<span data-ttu-id="d2fe7-150">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-150">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="d2fe7-151">underline</span><span class="sxs-lookup"><span data-stu-id="d2fe7-151">underline</span></span>|<span data-ttu-id="d2fe7-152">string</span><span class="sxs-lookup"><span data-stu-id="d2fe7-152">string</span></span>|<span data-ttu-id="d2fe7-p106">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="d2fe7-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2fe7-155">Response</span></span>

<span data-ttu-id="d2fe7-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [workbookChartFont](../resources/workbookchartfont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-156">If successful, this method returns a `200 OK` response code and updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2fe7-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2fe7-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2fe7-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2fe7-158">Request</span></span>
<span data-ttu-id="d2fe7-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2fe7-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2fe7-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d2fe7-161">C#</span><span class="sxs-lookup"><span data-stu-id="d2fe7-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2fe7-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2fe7-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2fe7-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2fe7-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2fe7-164">Java</span><span class="sxs-lookup"><span data-stu-id="d2fe7-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2fe7-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2fe7-165">Response</span></span>
<span data-ttu-id="d2fe7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


