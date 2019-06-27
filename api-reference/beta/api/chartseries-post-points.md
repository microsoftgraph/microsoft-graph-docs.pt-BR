---
title: Criar ChartPoints
description: Use essa API para criar novos ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: afbe102f3fdf0cc1d6fee61744c5a568ed100375
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261527"
---
# <a name="create-chartpoint"></a><span data-ttu-id="8ca0f-103">Criar ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8ca0f-103">Create ChartPoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ca0f-104">Use esta API para criar um novo ChartPoint.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-104">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ca0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ca0f-105">Permissions</span></span>
<span data-ttu-id="8ca0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ca0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ca0f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ca0f-108">Permission type</span></span>      | <span data-ttu-id="8ca0f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ca0f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ca0f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ca0f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ca0f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ca0f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ca0f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ca0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ca0f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ca0f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ca0f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ca0f-114">Application</span></span> | <span data-ttu-id="8ca0f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ca0f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ca0f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="8ca0f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ca0f-117">Request headers</span></span>
| <span data-ttu-id="8ca0f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ca0f-118">Name</span></span>       | <span data-ttu-id="8ca0f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ca0f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ca0f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ca0f-120">Authorization</span></span>  | <span data-ttu-id="8ca0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ca0f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ca0f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ca0f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ca0f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ca0f-126">Request body</span></span>
<span data-ttu-id="8ca0f-127">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChartPoint](../resources/workbookchartpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="8ca0f-127">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8ca0f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ca0f-128">Response</span></span>

<span data-ttu-id="8ca0f-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-129">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ca0f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ca0f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ca0f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ca0f-131">Request</span></span>
<span data-ttu-id="8ca0f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="8ca0f-133">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChartPoint](../resources/workbookchartpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="8ca0f-133">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8ca0f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ca0f-134">Response</span></span>
<span data-ttu-id="8ca0f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ca0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8ca0f-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8ca0f-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8ca0f-139">C#</span><span class="sxs-lookup"><span data-stu-id="8ca0f-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chartpoints_from_chartseries-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ca0f-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ca0f-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chartpoints_from_chartseries-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8ca0f-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8ca0f-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chartpoints_from_chartseries-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseries-post-points.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chartseries-post-points.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartseries-post-points.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
