---
title: Atualizar rangefont
description: Atualize as propriedades do objeto rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7554c121eab155449417cd34984dced48ed537d6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573961"
---
# <a name="update-rangefont"></a><span data-ttu-id="01d58-103">Atualizar rangefont</span><span class="sxs-lookup"><span data-stu-id="01d58-103">Update rangefont</span></span>

<span data-ttu-id="01d58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01d58-105">Atualize as propriedades do objeto rangefont.</span><span class="sxs-lookup"><span data-stu-id="01d58-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="01d58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="01d58-106">Permissions</span></span>
<span data-ttu-id="01d58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d58-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01d58-109">Permission type</span></span>      | <span data-ttu-id="01d58-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01d58-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01d58-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01d58-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01d58-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01d58-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01d58-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01d58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01d58-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01d58-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01d58-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01d58-115">Application</span></span> | <span data-ttu-id="01d58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01d58-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01d58-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01d58-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/font
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/font
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/font
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="01d58-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="01d58-118">Optional request headers</span></span>
| <span data-ttu-id="01d58-119">Nome</span><span class="sxs-lookup"><span data-stu-id="01d58-119">Name</span></span>       | <span data-ttu-id="01d58-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="01d58-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="01d58-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="01d58-121">Authorization</span></span>  | <span data-ttu-id="01d58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01d58-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01d58-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01d58-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="01d58-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="01d58-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01d58-127">Request body</span></span>
<span data-ttu-id="01d58-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="01d58-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="01d58-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01d58-131">Property</span></span>     | <span data-ttu-id="01d58-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="01d58-132">Type</span></span>   |<span data-ttu-id="01d58-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="01d58-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01d58-134">bold</span><span class="sxs-lookup"><span data-stu-id="01d58-134">bold</span></span>|<span data-ttu-id="01d58-135">booliano</span><span class="sxs-lookup"><span data-stu-id="01d58-135">boolean</span></span>|<span data-ttu-id="01d58-136">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="01d58-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="01d58-137">color</span><span class="sxs-lookup"><span data-stu-id="01d58-137">color</span></span>|<span data-ttu-id="01d58-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01d58-138">string</span></span>|<span data-ttu-id="01d58-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="01d58-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="01d58-142">italic</span><span class="sxs-lookup"><span data-stu-id="01d58-142">italic</span></span>|<span data-ttu-id="01d58-143">booliano</span><span class="sxs-lookup"><span data-stu-id="01d58-143">boolean</span></span>|<span data-ttu-id="01d58-144">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="01d58-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="01d58-145">nome</span><span class="sxs-lookup"><span data-stu-id="01d58-145">name</span></span>|<span data-ttu-id="01d58-146">string</span><span class="sxs-lookup"><span data-stu-id="01d58-146">string</span></span>|<span data-ttu-id="01d58-147">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="01d58-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="01d58-148">size</span><span class="sxs-lookup"><span data-stu-id="01d58-148">size</span></span>|<span data-ttu-id="01d58-149">Double</span><span class="sxs-lookup"><span data-stu-id="01d58-149">double</span></span>|<span data-ttu-id="01d58-150">Font Size</span><span class="sxs-lookup"><span data-stu-id="01d58-150">Font size.</span></span>|
|<span data-ttu-id="01d58-151">underline</span><span class="sxs-lookup"><span data-stu-id="01d58-151">underline</span></span>|<span data-ttu-id="01d58-152">string</span><span class="sxs-lookup"><span data-stu-id="01d58-152">string</span></span>|<span data-ttu-id="01d58-p106">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="01d58-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="01d58-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d58-155">Response</span></span>

<span data-ttu-id="01d58-156">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [workbookRangeFont](../resources/workbookrangefont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01d58-156">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01d58-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01d58-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01d58-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01d58-158">Request</span></span>
<span data-ttu-id="01d58-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01d58-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01d58-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="01d58-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/font
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
# <a name="c"></a>[<span data-ttu-id="01d58-161">C#</span><span class="sxs-lookup"><span data-stu-id="01d58-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01d58-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01d58-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01d58-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01d58-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01d58-164">Java</span><span class="sxs-lookup"><span data-stu-id="01d58-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01d58-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d58-165">Response</span></span>
<span data-ttu-id="01d58-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01d58-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


