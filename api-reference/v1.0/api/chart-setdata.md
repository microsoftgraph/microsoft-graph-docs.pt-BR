---
title: 'Chart: setData'
description: Redefine os dados de origem do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b028ca325d4f047e7b13b46fa1edd33385827457
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272622"
---
# <a name="chart-setdata"></a><span data-ttu-id="bf2af-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="bf2af-103">Chart: setData</span></span>

<span data-ttu-id="bf2af-104">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="bf2af-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf2af-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf2af-105">Permissions</span></span>
<span data-ttu-id="bf2af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf2af-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf2af-108">Permission type</span></span>      | <span data-ttu-id="bf2af-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf2af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf2af-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf2af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bf2af-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf2af-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf2af-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf2af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf2af-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf2af-113">Not supported.</span></span>    |
|<span data-ttu-id="bf2af-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf2af-114">Application</span></span> | <span data-ttu-id="bf2af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf2af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf2af-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf2af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="bf2af-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf2af-117">Request headers</span></span>
| <span data-ttu-id="bf2af-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bf2af-118">Name</span></span>       | <span data-ttu-id="bf2af-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf2af-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf2af-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf2af-120">Authorization</span></span>  | <span data-ttu-id="bf2af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf2af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf2af-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bf2af-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf2af-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bf2af-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf2af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf2af-126">Request body</span></span>
<span data-ttu-id="bf2af-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf2af-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf2af-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bf2af-128">Parameter</span></span>    | <span data-ttu-id="bf2af-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf2af-129">Type</span></span>   |<span data-ttu-id="bf2af-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf2af-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2af-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="bf2af-131">sourceData</span></span>|<span data-ttu-id="bf2af-132">Json</span><span class="sxs-lookup"><span data-stu-id="bf2af-132">Json</span></span>|<span data-ttu-id="bf2af-133">O objeto Range correspondente aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="bf2af-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="bf2af-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="bf2af-134">seriesBy</span></span>|<span data-ttu-id="bf2af-135">string</span><span class="sxs-lookup"><span data-stu-id="bf2af-135">string</span></span>|<span data-ttu-id="bf2af-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bf2af-136">Optional.</span></span> <span data-ttu-id="bf2af-137">Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico.</span><span class="sxs-lookup"><span data-stu-id="bf2af-137">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="bf2af-138">Pode ser um dos seguintes: Automático (padrão), Linhas, Colunas.</span><span class="sxs-lookup"><span data-stu-id="bf2af-138">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="bf2af-139">Os valores possíveis são: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="bf2af-139">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="bf2af-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf2af-140">Response</span></span>

<span data-ttu-id="bf2af-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf2af-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf2af-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf2af-143">Example</span></span>
<span data-ttu-id="bf2af-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bf2af-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf2af-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf2af-145">Request</span></span>
<span data-ttu-id="bf2af-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf2af-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="bf2af-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf2af-147">Response</span></span>
<span data-ttu-id="bf2af-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf2af-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf2af-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bf2af-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf2af-150">C#</span><span class="sxs-lookup"><span data-stu-id="bf2af-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setdata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf2af-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf2af-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setdata-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bf2af-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bf2af-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setdata-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
