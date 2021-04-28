---
title: Atualizar rangefont
description: Atualize as propriedades do objeto rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 22e369ee178b28d64c0c755595b328ba6fc4fc58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049440"
---
# <a name="update-rangefont"></a><span data-ttu-id="e65bb-103">Atualizar rangefont</span><span class="sxs-lookup"><span data-stu-id="e65bb-103">Update rangefont</span></span>

<span data-ttu-id="e65bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e65bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e65bb-105">Atualize as propriedades do objeto rangefont.</span><span class="sxs-lookup"><span data-stu-id="e65bb-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e65bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e65bb-106">Permissions</span></span>
<span data-ttu-id="e65bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e65bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e65bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e65bb-109">Permission type</span></span>      | <span data-ttu-id="e65bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e65bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e65bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e65bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e65bb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e65bb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e65bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e65bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e65bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e65bb-114">Not supported.</span></span>    |
|<span data-ttu-id="e65bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e65bb-115">Application</span></span> | <span data-ttu-id="e65bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e65bb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e65bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e65bb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/font
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/font
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="request-headers"></a><span data-ttu-id="e65bb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e65bb-118">Request headers</span></span>
| <span data-ttu-id="e65bb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e65bb-119">Name</span></span>       | <span data-ttu-id="e65bb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e65bb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e65bb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e65bb-121">Authorization</span></span>  | <span data-ttu-id="e65bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e65bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e65bb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e65bb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e65bb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e65bb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e65bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e65bb-127">Request body</span></span>
<span data-ttu-id="e65bb-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e65bb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e65bb-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e65bb-131">Property</span></span>     | <span data-ttu-id="e65bb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e65bb-132">Type</span></span>   |<span data-ttu-id="e65bb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e65bb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65bb-134">bold</span><span class="sxs-lookup"><span data-stu-id="e65bb-134">bold</span></span>|<span data-ttu-id="e65bb-135">booliano</span><span class="sxs-lookup"><span data-stu-id="e65bb-135">boolean</span></span>|<span data-ttu-id="e65bb-136">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="e65bb-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="e65bb-137">color</span><span class="sxs-lookup"><span data-stu-id="e65bb-137">color</span></span>|<span data-ttu-id="e65bb-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e65bb-138">string</span></span>|<span data-ttu-id="e65bb-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="e65bb-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="e65bb-142">italic</span><span class="sxs-lookup"><span data-stu-id="e65bb-142">italic</span></span>|<span data-ttu-id="e65bb-143">booliano</span><span class="sxs-lookup"><span data-stu-id="e65bb-143">boolean</span></span>|<span data-ttu-id="e65bb-144">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="e65bb-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="e65bb-145">nome</span><span class="sxs-lookup"><span data-stu-id="e65bb-145">name</span></span>|<span data-ttu-id="e65bb-146">string</span><span class="sxs-lookup"><span data-stu-id="e65bb-146">string</span></span>|<span data-ttu-id="e65bb-147">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="e65bb-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="e65bb-148">size</span><span class="sxs-lookup"><span data-stu-id="e65bb-148">size</span></span>|<span data-ttu-id="e65bb-149">Double</span><span class="sxs-lookup"><span data-stu-id="e65bb-149">double</span></span>|<span data-ttu-id="e65bb-150">Font Size</span><span class="sxs-lookup"><span data-stu-id="e65bb-150">Font size.</span></span>|
|<span data-ttu-id="e65bb-151">underline</span><span class="sxs-lookup"><span data-stu-id="e65bb-151">underline</span></span>|<span data-ttu-id="e65bb-152">string</span><span class="sxs-lookup"><span data-stu-id="e65bb-152">string</span></span>|<span data-ttu-id="e65bb-153">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="e65bb-153">Type of underline applied to the font.</span></span> <span data-ttu-id="e65bb-154">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="e65bb-154">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="e65bb-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65bb-155">Response</span></span>

<span data-ttu-id="e65bb-156">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookRangeFont](../resources/rangefont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e65bb-156">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e65bb-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e65bb-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e65bb-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e65bb-158">Request</span></span>
<span data-ttu-id="e65bb-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e65bb-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e65bb-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e65bb-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/font
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
# <a name="c"></a>[<span data-ttu-id="e65bb-161">C#</span><span class="sxs-lookup"><span data-stu-id="e65bb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e65bb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e65bb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e65bb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e65bb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e65bb-164">Java</span><span class="sxs-lookup"><span data-stu-id="e65bb-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e65bb-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65bb-165">Response</span></span>
<span data-ttu-id="e65bb-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e65bb-166">Here is an example of the response.</span></span> <span data-ttu-id="e65bb-167">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e65bb-167">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

