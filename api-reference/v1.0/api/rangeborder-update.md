---
title: Atualizar rangeborder
description: Atualize as propriedades do objeto rangeborder.
author: lumine2008
ms.openlocfilehash: ed9b2e5fa6b3d4a1dd3c227160eb71435e9a3817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311939"
---
# <a name="update-rangeborder"></a><span data-ttu-id="ca592-103">Atualizar rangeborder</span><span class="sxs-lookup"><span data-stu-id="ca592-103">Update rangeborder</span></span>

<span data-ttu-id="ca592-104">Atualize as propriedades do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="ca592-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca592-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca592-105">Permissions</span></span>
<span data-ttu-id="ca592-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca592-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca592-108">Permission type</span></span>      | <span data-ttu-id="ca592-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca592-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca592-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca592-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ca592-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca592-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca592-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca592-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca592-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca592-113">Not supported.</span></span>    |
|<span data-ttu-id="ca592-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca592-114">Application</span></span> | <span data-ttu-id="ca592-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca592-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca592-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca592-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ca592-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ca592-117">Optional request headers</span></span>
| <span data-ttu-id="ca592-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ca592-118">Name</span></span>       | <span data-ttu-id="ca592-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca592-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ca592-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca592-120">Authorization</span></span>  | <span data-ttu-id="ca592-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca592-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca592-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ca592-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ca592-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ca592-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca592-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca592-126">Request body</span></span>
<span data-ttu-id="ca592-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ca592-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ca592-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca592-130">Property</span></span>     | <span data-ttu-id="ca592-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca592-131">Type</span></span>   |<span data-ttu-id="ca592-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca592-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca592-133">color</span><span class="sxs-lookup"><span data-stu-id="ca592-133">color</span></span>|<span data-ttu-id="ca592-134">string</span><span class="sxs-lookup"><span data-stu-id="ca592-134">string</span></span>|<span data-ttu-id="ca592-135">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="ca592-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="ca592-136">style</span><span class="sxs-lookup"><span data-stu-id="ca592-136">style</span></span>|<span data-ttu-id="ca592-137">string</span><span class="sxs-lookup"><span data-stu-id="ca592-137">string</span></span>|<span data-ttu-id="ca592-138">Uma das constantes de estilo de linha, especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="ca592-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="ca592-139">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="ca592-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="ca592-140">weight</span><span class="sxs-lookup"><span data-stu-id="ca592-140">weight</span></span>|<span data-ttu-id="ca592-141">string</span><span class="sxs-lookup"><span data-stu-id="ca592-141">string</span></span>|<span data-ttu-id="ca592-142">Especifica o peso da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="ca592-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="ca592-143">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="ca592-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="ca592-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca592-144">Response</span></span>

<span data-ttu-id="ca592-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookRangeBorder](../resources/rangeborder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca592-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca592-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca592-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca592-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca592-147">Request</span></span>
<span data-ttu-id="ca592-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca592-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ca592-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca592-149">Response</span></span>
<span data-ttu-id="ca592-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca592-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->