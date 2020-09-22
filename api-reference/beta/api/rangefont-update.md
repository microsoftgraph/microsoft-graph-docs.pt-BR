---
title: Atualizar rangefont
description: Atualize as propriedades do objeto rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 635d1e7304fa1296dd1f1af9c348c11db4b65725
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034284"
---
# <a name="update-rangefont"></a><span data-ttu-id="3b703-103">Atualizar rangefont</span><span class="sxs-lookup"><span data-stu-id="3b703-103">Update rangefont</span></span>

<span data-ttu-id="3b703-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b703-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b703-105">Atualize as propriedades do objeto rangefont.</span><span class="sxs-lookup"><span data-stu-id="3b703-105">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b703-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b703-106">Permissions</span></span>
<span data-ttu-id="3b703-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b703-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b703-109">Permission type</span></span>      | <span data-ttu-id="3b703-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b703-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b703-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b703-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b703-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b703-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b703-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b703-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b703-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b703-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b703-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b703-115">Application</span></span> | <span data-ttu-id="3b703-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b703-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b703-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b703-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="3b703-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3b703-118">Optional request headers</span></span>
| <span data-ttu-id="3b703-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3b703-119">Name</span></span>       | <span data-ttu-id="3b703-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b703-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3b703-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b703-121">Authorization</span></span>  | <span data-ttu-id="3b703-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b703-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b703-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3b703-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b703-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3b703-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b703-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b703-127">Request body</span></span>
<span data-ttu-id="3b703-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3b703-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b703-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b703-131">Property</span></span>     | <span data-ttu-id="3b703-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b703-132">Type</span></span>   |<span data-ttu-id="3b703-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b703-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b703-134">bold</span><span class="sxs-lookup"><span data-stu-id="3b703-134">bold</span></span>|<span data-ttu-id="3b703-135">booliano</span><span class="sxs-lookup"><span data-stu-id="3b703-135">boolean</span></span>|<span data-ttu-id="3b703-136">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="3b703-136">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3b703-137">color</span><span class="sxs-lookup"><span data-stu-id="3b703-137">color</span></span>|<span data-ttu-id="3b703-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b703-138">string</span></span>|<span data-ttu-id="3b703-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="3b703-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3b703-142">italic</span><span class="sxs-lookup"><span data-stu-id="3b703-142">italic</span></span>|<span data-ttu-id="3b703-143">booliano</span><span class="sxs-lookup"><span data-stu-id="3b703-143">boolean</span></span>|<span data-ttu-id="3b703-144">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="3b703-144">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3b703-145">nome</span><span class="sxs-lookup"><span data-stu-id="3b703-145">name</span></span>|<span data-ttu-id="3b703-146">string</span><span class="sxs-lookup"><span data-stu-id="3b703-146">string</span></span>|<span data-ttu-id="3b703-147">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="3b703-147">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3b703-148">size</span><span class="sxs-lookup"><span data-stu-id="3b703-148">size</span></span>|<span data-ttu-id="3b703-149">Double</span><span class="sxs-lookup"><span data-stu-id="3b703-149">double</span></span>|<span data-ttu-id="3b703-150">Font Size</span><span class="sxs-lookup"><span data-stu-id="3b703-150">Font size.</span></span>|
|<span data-ttu-id="3b703-151">underline</span><span class="sxs-lookup"><span data-stu-id="3b703-151">underline</span></span>|<span data-ttu-id="3b703-152">string</span><span class="sxs-lookup"><span data-stu-id="3b703-152">string</span></span>|<span data-ttu-id="3b703-p106">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="3b703-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="3b703-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b703-155">Response</span></span>

<span data-ttu-id="3b703-156">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookRangeFont](../resources/workbookrangefont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b703-156">If successful, this method returns a `200 OK` response code and updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b703-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b703-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b703-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b703-158">Request</span></span>
<span data-ttu-id="3b703-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b703-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b703-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b703-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3b703-161">C#</span><span class="sxs-lookup"><span data-stu-id="3b703-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b703-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b703-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b703-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b703-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3b703-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b703-164">Response</span></span>
<span data-ttu-id="3b703-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b703-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


