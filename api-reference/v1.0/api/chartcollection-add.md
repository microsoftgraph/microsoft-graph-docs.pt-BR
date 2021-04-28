---
title: 'ChartCollection: add'
description: Cria um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a2550ba3c86ea7c714bd7eaa6526e2a96ca3e236
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053269"
---
# <a name="chartcollection-add"></a><span data-ttu-id="52437-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="52437-103">ChartCollection: add</span></span>

<span data-ttu-id="52437-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52437-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52437-105">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="52437-105">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="52437-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52437-106">Permissions</span></span>
<span data-ttu-id="52437-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52437-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52437-109">Permission type</span></span>      | <span data-ttu-id="52437-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52437-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52437-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52437-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52437-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52437-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52437-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52437-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52437-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52437-114">Not supported.</span></span>    |
|<span data-ttu-id="52437-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52437-115">Application</span></span> | <span data-ttu-id="52437-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52437-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52437-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52437-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="52437-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52437-118">Request headers</span></span>
| <span data-ttu-id="52437-119">Nome</span><span class="sxs-lookup"><span data-stu-id="52437-119">Name</span></span>       | <span data-ttu-id="52437-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52437-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52437-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52437-121">Authorization</span></span>  | <span data-ttu-id="52437-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52437-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52437-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52437-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="52437-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="52437-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52437-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52437-127">Request body</span></span>
<span data-ttu-id="52437-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52437-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52437-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52437-129">Parameter</span></span>    | <span data-ttu-id="52437-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="52437-130">Type</span></span>   |<span data-ttu-id="52437-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="52437-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52437-132">type</span><span class="sxs-lookup"><span data-stu-id="52437-132">type</span></span>|<span data-ttu-id="52437-133">string</span><span class="sxs-lookup"><span data-stu-id="52437-133">string</span></span>|<span data-ttu-id="52437-134">Representa o tipo de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="52437-134">Represents the type of a chart.</span></span>  <span data-ttu-id="52437-135">Os valores possíveis são: `ColumnClustered` , , , , , , , , , `ColumnStacked` , , `ColumnStacked100` , , , `BarClustered` , `BarStacked` `BarStacked100` `LineStacked` `LineStacked100` `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100` `PieOfPie` `etc.` .</span><span class="sxs-lookup"><span data-stu-id="52437-135">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="52437-136">sourceData</span><span class="sxs-lookup"><span data-stu-id="52437-136">sourceData</span></span>|<span data-ttu-id="52437-137">Json</span><span class="sxs-lookup"><span data-stu-id="52437-137">Json</span></span>|<span data-ttu-id="52437-138">O objeto Range correspondente aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="52437-138">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="52437-139">seriesBy</span><span class="sxs-lookup"><span data-stu-id="52437-139">seriesBy</span></span>|<span data-ttu-id="52437-140">string</span><span class="sxs-lookup"><span data-stu-id="52437-140">string</span></span>|<span data-ttu-id="52437-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="52437-141">Optional.</span></span> <span data-ttu-id="52437-142">Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico.</span><span class="sxs-lookup"><span data-stu-id="52437-142">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="52437-143">Os valores possíveis são: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="52437-143">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="52437-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="52437-144">Response</span></span>

<span data-ttu-id="52437-145">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52437-145">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52437-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52437-146">Example</span></span>
<span data-ttu-id="52437-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="52437-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52437-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52437-148">Request</span></span>
<span data-ttu-id="52437-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52437-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52437-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="52437-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="52437-151">C#</span><span class="sxs-lookup"><span data-stu-id="52437-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52437-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52437-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52437-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52437-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52437-154">Java</span><span class="sxs-lookup"><span data-stu-id="52437-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="52437-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="52437-155">Response</span></span>
<span data-ttu-id="52437-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52437-156">Here is an example of the response.</span></span> <span data-ttu-id="52437-157">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52437-157">Note: The response object shown here might be shortened for readability.</span></span>
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

