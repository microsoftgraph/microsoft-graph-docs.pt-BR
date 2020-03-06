---
title: Atualizar rangeborder
description: Atualize as propriedades do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3cce44c14eb9253bc391014a555966e1f4c50a2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510547"
---
# <a name="update-rangeborder"></a><span data-ttu-id="46b77-103">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="46b77-103">Update rangeborder</span></span>

<span data-ttu-id="46b77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46b77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46b77-105">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="46b77-105">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="46b77-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46b77-106">Permissions</span></span>
<span data-ttu-id="46b77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b77-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46b77-109">Permission type</span></span>      | <span data-ttu-id="46b77-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46b77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46b77-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46b77-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46b77-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b77-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46b77-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46b77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46b77-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46b77-114">Not supported.</span></span>    |
|<span data-ttu-id="46b77-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46b77-115">Application</span></span> | <span data-ttu-id="46b77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46b77-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46b77-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46b77-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="46b77-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="46b77-118">Optional request headers</span></span>
| <span data-ttu-id="46b77-119">Nome</span><span class="sxs-lookup"><span data-stu-id="46b77-119">Name</span></span>       | <span data-ttu-id="46b77-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b77-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="46b77-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="46b77-121">Authorization</span></span>  | <span data-ttu-id="46b77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46b77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46b77-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="46b77-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="46b77-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="46b77-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46b77-127">Request body</span></span>
<span data-ttu-id="46b77-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="46b77-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46b77-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46b77-131">Property</span></span>     | <span data-ttu-id="46b77-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="46b77-132">Type</span></span>   |<span data-ttu-id="46b77-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b77-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46b77-134">color</span><span class="sxs-lookup"><span data-stu-id="46b77-134">color</span></span>|<span data-ttu-id="46b77-135">string</span><span class="sxs-lookup"><span data-stu-id="46b77-135">string</span></span>|<span data-ttu-id="46b77-136">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="46b77-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="46b77-137">style</span><span class="sxs-lookup"><span data-stu-id="46b77-137">style</span></span>|<span data-ttu-id="46b77-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46b77-138">string</span></span>|<span data-ttu-id="46b77-139">Uma das constantes de estilo de linha especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="46b77-139">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="46b77-140">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="46b77-140">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="46b77-141">weight</span><span class="sxs-lookup"><span data-stu-id="46b77-141">weight</span></span>|<span data-ttu-id="46b77-142">string</span><span class="sxs-lookup"><span data-stu-id="46b77-142">string</span></span>|<span data-ttu-id="46b77-143">Especifica a espessura da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="46b77-143">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="46b77-144">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="46b77-144">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="46b77-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b77-145">Response</span></span>

<span data-ttu-id="46b77-146">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookRangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b77-146">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46b77-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46b77-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46b77-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46b77-148">Request</span></span>
<span data-ttu-id="46b77-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b77-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46b77-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="46b77-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="46b77-151">C#</span><span class="sxs-lookup"><span data-stu-id="46b77-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46b77-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46b77-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46b77-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46b77-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46b77-154">Java</span><span class="sxs-lookup"><span data-stu-id="46b77-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeborder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="46b77-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b77-155">Response</span></span>
<span data-ttu-id="46b77-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46b77-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
