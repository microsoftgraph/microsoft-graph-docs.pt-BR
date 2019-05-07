---
title: Atualizar workbookChartAxisTitle
description: Atualize as propriedades do objeto workbookchartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4667d3dc1cc2daa24c8a66c8ead9c3c71fa208e8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635621"
---
# <a name="update-workbookchartaxistitle"></a><span data-ttu-id="74290-103">Atualizar workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="74290-103">Update workbookChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74290-104">Atualize as propriedades do objeto workbookChartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="74290-104">Update the properties of workbookChartAxisTitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74290-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="74290-105">Permissions</span></span>
<span data-ttu-id="74290-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74290-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74290-108">Permission type</span></span>      | <span data-ttu-id="74290-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74290-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74290-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74290-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74290-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74290-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74290-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74290-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74290-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74290-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74290-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74290-114">Application</span></span> | <span data-ttu-id="74290-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74290-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74290-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74290-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="74290-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="74290-117">Optional request headers</span></span>
| <span data-ttu-id="74290-118">Nome</span><span class="sxs-lookup"><span data-stu-id="74290-118">Name</span></span>       | <span data-ttu-id="74290-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="74290-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="74290-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="74290-120">Authorization</span></span>  | <span data-ttu-id="74290-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74290-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74290-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74290-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="74290-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="74290-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74290-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74290-126">Request body</span></span>
<span data-ttu-id="74290-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="74290-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74290-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74290-130">Property</span></span>     | <span data-ttu-id="74290-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="74290-131">Type</span></span>   |<span data-ttu-id="74290-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="74290-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74290-133">texto</span><span class="sxs-lookup"><span data-stu-id="74290-133">text</span></span>|<span data-ttu-id="74290-134">string</span><span class="sxs-lookup"><span data-stu-id="74290-134">string</span></span>|<span data-ttu-id="74290-135">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="74290-135">Represents the axis title.</span></span>|
|<span data-ttu-id="74290-136">visible</span><span class="sxs-lookup"><span data-stu-id="74290-136">visible</span></span>|<span data-ttu-id="74290-137">booliano</span><span class="sxs-lookup"><span data-stu-id="74290-137">boolean</span></span>|<span data-ttu-id="74290-138">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="74290-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="74290-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="74290-139">Response</span></span>

<span data-ttu-id="74290-140">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74290-140">If successful, this method returns a `200 OK` response code and updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74290-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74290-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74290-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74290-142">Request</span></span>
<span data-ttu-id="74290-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74290-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="74290-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="74290-144">Response</span></span>
<span data-ttu-id="74290-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74290-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74290-148">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="74290-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74290-149">Basic</span><span class="sxs-lookup"><span data-stu-id="74290-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartaxistitle-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74290-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74290-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartaxistitle-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
