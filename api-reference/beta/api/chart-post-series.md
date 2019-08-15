---
title: Criar ChartSeries
description: Use essa API para criar novas ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c97e468bdadb1980b168d2f15a4a21f340b88762
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418628"
---
# <a name="create-chartseries"></a><span data-ttu-id="c48cf-103">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c48cf-103">Create ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c48cf-104">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="c48cf-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="c48cf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c48cf-105">Permissions</span></span>
<span data-ttu-id="c48cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c48cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c48cf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c48cf-108">Permission type</span></span>      | <span data-ttu-id="c48cf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c48cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c48cf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c48cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c48cf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c48cf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c48cf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c48cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c48cf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c48cf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c48cf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c48cf-114">Application</span></span> | <span data-ttu-id="c48cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c48cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c48cf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c48cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="c48cf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c48cf-117">Request headers</span></span>
| <span data-ttu-id="c48cf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c48cf-118">Name</span></span>       | <span data-ttu-id="c48cf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c48cf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c48cf-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c48cf-120">Authorization</span></span>  | <span data-ttu-id="c48cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c48cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c48cf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c48cf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c48cf-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c48cf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c48cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c48cf-126">Request body</span></span>
<span data-ttu-id="c48cf-127">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChartSeries](../resources/workbookchartseries.md) .</span><span class="sxs-lookup"><span data-stu-id="c48cf-127">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c48cf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c48cf-128">Response</span></span>

<span data-ttu-id="c48cf-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookChartSeries](../resources/workbookchartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c48cf-129">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c48cf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c48cf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c48cf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c48cf-131">Request</span></span>
<span data-ttu-id="c48cf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c48cf-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c48cf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c48cf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c48cf-134">C#</span><span class="sxs-lookup"><span data-stu-id="c48cf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c48cf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c48cf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c48cf-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c48cf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c48cf-137">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChartSeries](../resources/workbookchartseries.md) .</span><span class="sxs-lookup"><span data-stu-id="c48cf-137">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c48cf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c48cf-138">Response</span></span>
<span data-ttu-id="c48cf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c48cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
