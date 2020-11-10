---
title: 'workbookChartCollection: Adicionar'
description: Cria um novo workbookChart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c7d5911190fe41e0afa7a4d158ba7a81bd955d68
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958847"
---
# <a name="workbookchartcollection-add"></a><span data-ttu-id="aa0d6-103">workbookChartCollection: Adicionar</span><span class="sxs-lookup"><span data-stu-id="aa0d6-103">workbookChartCollection: add</span></span>

<span data-ttu-id="aa0d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa0d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa0d6-105">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-105">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa0d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa0d6-106">Permissions</span></span>
<span data-ttu-id="aa0d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa0d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa0d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa0d6-109">Permission type</span></span>      | <span data-ttu-id="aa0d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa0d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa0d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa0d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa0d6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa0d6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa0d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa0d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa0d6-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa0d6-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa0d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa0d6-115">Application</span></span> | <span data-ttu-id="aa0d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa0d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="aa0d6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa0d6-118">Request headers</span></span>
| <span data-ttu-id="aa0d6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="aa0d6-119">Name</span></span>       | <span data-ttu-id="aa0d6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa0d6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa0d6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa0d6-121">Authorization</span></span>  | <span data-ttu-id="aa0d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa0d6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aa0d6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa0d6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa0d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa0d6-127">Request body</span></span>
<span data-ttu-id="aa0d6-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aa0d6-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aa0d6-129">Parameter</span></span>    | <span data-ttu-id="aa0d6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa0d6-130">Type</span></span>   |<span data-ttu-id="aa0d6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa0d6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa0d6-132">type</span><span class="sxs-lookup"><span data-stu-id="aa0d6-132">type</span></span>|<span data-ttu-id="aa0d6-133">string</span><span class="sxs-lookup"><span data-stu-id="aa0d6-133">string</span></span>|<span data-ttu-id="aa0d6-134">Representa o tipo de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-134">Represents the type of a chart.</span></span>  <span data-ttu-id="aa0d6-135">Os valores possíveis são: `ColumnClustered` , `ColumnStacked` , `ColumnStacked100` , `BarClustered` , `BarStacked` , `BarStacked100` , `LineStacked` , `LineStacked100` , `LineMarkers` , `LineMarkersStacked` , `LineMarkersStacked100` , `PieOfPie` , `etc.` .</span><span class="sxs-lookup"><span data-stu-id="aa0d6-135">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="aa0d6-136">sourceData</span><span class="sxs-lookup"><span data-stu-id="aa0d6-136">sourceData</span></span>|<span data-ttu-id="aa0d6-137">Json</span><span class="sxs-lookup"><span data-stu-id="aa0d6-137">Json</span></span>|<span data-ttu-id="aa0d6-138">O objeto Range correspondente aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-138">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="aa0d6-139">seriesBy</span><span class="sxs-lookup"><span data-stu-id="aa0d6-139">seriesBy</span></span>|<span data-ttu-id="aa0d6-140">string</span><span class="sxs-lookup"><span data-stu-id="aa0d6-140">string</span></span>|<span data-ttu-id="aa0d6-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-141">Optional.</span></span> <span data-ttu-id="aa0d6-142">Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-142">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="aa0d6-143">Os valores possíveis são: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-143">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="aa0d6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa0d6-144">Response</span></span>

<span data-ttu-id="aa0d6-145">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-145">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa0d6-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa0d6-146">Example</span></span>
<span data-ttu-id="aa0d6-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aa0d6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa0d6-148">Request</span></span>
<span data-ttu-id="aa0d6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa0d6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0d6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```
# <a name="c"></a>[<span data-ttu-id="aa0d6-151">C#</span><span class="sxs-lookup"><span data-stu-id="aa0d6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa0d6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa0d6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa0d6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa0d6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa0d6-154">Java</span><span class="sxs-lookup"><span data-stu-id="aa0d6-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa0d6-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa0d6-155">Response</span></span>
<span data-ttu-id="aa0d6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa0d6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


