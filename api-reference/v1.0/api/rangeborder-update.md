---
title: Atualizar rangeborder
description: Atualize as propriedades do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 85cb2ad1057369b46c47780aa4d0f8fb68bf18c7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053906"
---
# <a name="update-rangeborder"></a><span data-ttu-id="54c00-103">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="54c00-103">Update rangeborder</span></span>

<span data-ttu-id="54c00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54c00-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54c00-105">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="54c00-105">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54c00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54c00-106">Permissions</span></span>
<span data-ttu-id="54c00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54c00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54c00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54c00-109">Permission type</span></span>      | <span data-ttu-id="54c00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54c00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54c00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54c00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54c00-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54c00-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="54c00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54c00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54c00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54c00-114">Not supported.</span></span>    |
|<span data-ttu-id="54c00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54c00-115">Application</span></span> | <span data-ttu-id="54c00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54c00-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54c00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54c00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="54c00-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="54c00-118">Optional request headers</span></span>
| <span data-ttu-id="54c00-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54c00-119">Name</span></span>       | <span data-ttu-id="54c00-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54c00-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="54c00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54c00-121">Authorization</span></span>  | <span data-ttu-id="54c00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54c00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54c00-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="54c00-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="54c00-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="54c00-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54c00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54c00-127">Request body</span></span>
<span data-ttu-id="54c00-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="54c00-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="54c00-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54c00-131">Property</span></span>     | <span data-ttu-id="54c00-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="54c00-132">Type</span></span>   |<span data-ttu-id="54c00-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="54c00-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54c00-134">color</span><span class="sxs-lookup"><span data-stu-id="54c00-134">color</span></span>|<span data-ttu-id="54c00-135">string</span><span class="sxs-lookup"><span data-stu-id="54c00-135">string</span></span>|<span data-ttu-id="54c00-136">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="54c00-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="54c00-137">style</span><span class="sxs-lookup"><span data-stu-id="54c00-137">style</span></span>|<span data-ttu-id="54c00-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54c00-138">string</span></span>|<span data-ttu-id="54c00-139">Uma das constantes de estilo de linha especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="54c00-139">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="54c00-140">Os valores possíveis são: `None` , , , , , , , , `Continuous` `Dash` `DashDot` `DashDotDot` `Dot` `Double` `SlantDashDot` .</span><span class="sxs-lookup"><span data-stu-id="54c00-140">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="54c00-141">weight</span><span class="sxs-lookup"><span data-stu-id="54c00-141">weight</span></span>|<span data-ttu-id="54c00-142">string</span><span class="sxs-lookup"><span data-stu-id="54c00-142">string</span></span>|<span data-ttu-id="54c00-143">Especifica a espessura da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="54c00-143">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="54c00-144">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="54c00-144">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="54c00-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="54c00-145">Response</span></span>

<span data-ttu-id="54c00-146">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookRangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54c00-146">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54c00-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54c00-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54c00-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54c00-148">Request</span></span>
<span data-ttu-id="54c00-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54c00-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54c00-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="54c00-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="c"></a>[<span data-ttu-id="54c00-151">C#</span><span class="sxs-lookup"><span data-stu-id="54c00-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54c00-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54c00-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54c00-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54c00-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54c00-154">Java</span><span class="sxs-lookup"><span data-stu-id="54c00-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeborder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54c00-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="54c00-155">Response</span></span>
<span data-ttu-id="54c00-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54c00-156">Here is an example of the response.</span></span> <span data-ttu-id="54c00-157">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="54c00-157">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

