---
title: 'ChartCollection: add'
description: Cria um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ae3526730db4bba39e7f6b1e08cf6408a73fdf14
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443494"
---
# <a name="chartcollection-add"></a><span data-ttu-id="aacea-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="aacea-103">ChartCollection: add</span></span>

<span data-ttu-id="aacea-104">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="aacea-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="aacea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aacea-105">Permissions</span></span>
<span data-ttu-id="aacea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aacea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aacea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aacea-108">Permission type</span></span>      | <span data-ttu-id="aacea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aacea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aacea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aacea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aacea-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aacea-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aacea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aacea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aacea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aacea-113">Not supported.</span></span>    |
|<span data-ttu-id="aacea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aacea-114">Application</span></span> | <span data-ttu-id="aacea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aacea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aacea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aacea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="aacea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aacea-117">Request headers</span></span>
| <span data-ttu-id="aacea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="aacea-118">Name</span></span>       | <span data-ttu-id="aacea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aacea-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aacea-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aacea-120">Authorization</span></span>  | <span data-ttu-id="aacea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aacea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aacea-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aacea-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="aacea-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="aacea-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aacea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aacea-126">Request body</span></span>
<span data-ttu-id="aacea-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aacea-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aacea-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aacea-128">Parameter</span></span>    | <span data-ttu-id="aacea-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="aacea-129">Type</span></span>   |<span data-ttu-id="aacea-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aacea-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aacea-131">type</span><span class="sxs-lookup"><span data-stu-id="aacea-131">type</span></span>|<span data-ttu-id="aacea-132">string</span><span class="sxs-lookup"><span data-stu-id="aacea-132">string</span></span>|<span data-ttu-id="aacea-133">Representa o tipo de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="aacea-133">Represents the type of a chart.</span></span>  <span data-ttu-id="aacea-134">Os valores possíveis são: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="aacea-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="aacea-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="aacea-135">sourceData</span></span>|<span data-ttu-id="aacea-136">Json</span><span class="sxs-lookup"><span data-stu-id="aacea-136">Json</span></span>|<span data-ttu-id="aacea-137">O objeto Range correspondente aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="aacea-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="aacea-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="aacea-138">seriesBy</span></span>|<span data-ttu-id="aacea-139">string</span><span class="sxs-lookup"><span data-stu-id="aacea-139">string</span></span>|<span data-ttu-id="aacea-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aacea-140">Optional.</span></span> <span data-ttu-id="aacea-141">Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico.</span><span class="sxs-lookup"><span data-stu-id="aacea-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="aacea-142">Os valores possíveis são: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="aacea-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="aacea-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="aacea-143">Response</span></span>

<span data-ttu-id="aacea-144">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aacea-144">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aacea-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aacea-145">Example</span></span>
<span data-ttu-id="aacea-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="aacea-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aacea-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aacea-147">Request</span></span>
<span data-ttu-id="aacea-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aacea-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aacea-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="aacea-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aacea-150">C#</span><span class="sxs-lookup"><span data-stu-id="aacea-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aacea-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="aacea-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aacea-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="aacea-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aacea-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="aacea-153">Response</span></span>
<span data-ttu-id="aacea-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aacea-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
