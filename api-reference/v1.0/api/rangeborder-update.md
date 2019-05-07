---
title: Atualizar rangeborder
description: Atualize as propriedades do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a850d4db197906b7c1c5f7986166a85143ddf544
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607982"
---
# <a name="update-rangeborder"></a><span data-ttu-id="e5c2c-103">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="e5c2c-103">Update rangeborder</span></span>

<span data-ttu-id="e5c2c-104">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5c2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5c2c-105">Permissions</span></span>
<span data-ttu-id="e5c2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5c2c-108">Permission type</span></span>      | <span data-ttu-id="e5c2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5c2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5c2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5c2c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5c2c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5c2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5c2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c2c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-113">Not supported.</span></span>    |
|<span data-ttu-id="e5c2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5c2c-114">Application</span></span> | <span data-ttu-id="e5c2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5c2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5c2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e5c2c-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e5c2c-117">Optional request headers</span></span>
| <span data-ttu-id="e5c2c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e5c2c-118">Name</span></span>       | <span data-ttu-id="e5c2c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5c2c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e5c2c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5c2c-120">Authorization</span></span>  | <span data-ttu-id="e5c2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5c2c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5c2c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5c2c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5c2c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c2c-126">Request body</span></span>
<span data-ttu-id="e5c2c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5c2c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5c2c-130">Property</span></span>     | <span data-ttu-id="e5c2c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5c2c-131">Type</span></span>   |<span data-ttu-id="e5c2c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5c2c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5c2c-133">color</span><span class="sxs-lookup"><span data-stu-id="e5c2c-133">color</span></span>|<span data-ttu-id="e5c2c-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5c2c-134">string</span></span>|<span data-ttu-id="e5c2c-135">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="e5c2c-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="e5c2c-136">style</span><span class="sxs-lookup"><span data-stu-id="e5c2c-136">style</span></span>|<span data-ttu-id="e5c2c-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5c2c-137">string</span></span>|<span data-ttu-id="e5c2c-138">Uma das constantes de estilo de linha especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="e5c2c-139">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="e5c2c-140">weight</span><span class="sxs-lookup"><span data-stu-id="e5c2c-140">weight</span></span>|<span data-ttu-id="e5c2c-141">string</span><span class="sxs-lookup"><span data-stu-id="e5c2c-141">string</span></span>|<span data-ttu-id="e5c2c-142">Especifica a espessura da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="e5c2c-143">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="e5c2c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5c2c-144">Response</span></span>

<span data-ttu-id="e5c2c-145">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookRangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5c2c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5c2c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5c2c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c2c-147">Request</span></span>
<span data-ttu-id="e5c2c-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e5c2c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5c2c-149">Response</span></span>
<span data-ttu-id="e5c2c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5c2c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e5c2c-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e5c2c-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e5c2c-154">Basic</span><span class="sxs-lookup"><span data-stu-id="e5c2c-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeborder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5c2c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5c2c-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeborder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeborder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeborder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
