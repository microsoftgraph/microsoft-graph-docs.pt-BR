---
title: Criar ChartSeries
description: Use essa API para criar novas ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 426555d2d68620a38ff3c34bf25881c66ecaabe5
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574787"
---
# <a name="create-chartseries"></a><span data-ttu-id="415b0-103">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="415b0-103">Create ChartSeries</span></span>

<span data-ttu-id="415b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="415b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="415b0-105">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="415b0-105">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="415b0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="415b0-106">Permissions</span></span>
<span data-ttu-id="415b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="415b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="415b0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="415b0-109">Permission type</span></span>      | <span data-ttu-id="415b0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="415b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="415b0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="415b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="415b0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="415b0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="415b0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="415b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="415b0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="415b0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="415b0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="415b0-115">Application</span></span> | <span data-ttu-id="415b0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="415b0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="415b0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="415b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="415b0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="415b0-118">Request headers</span></span>
| <span data-ttu-id="415b0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="415b0-119">Name</span></span>       | <span data-ttu-id="415b0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="415b0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="415b0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="415b0-121">Authorization</span></span>  | <span data-ttu-id="415b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="415b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="415b0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="415b0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="415b0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="415b0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="415b0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="415b0-127">Request body</span></span>
<span data-ttu-id="415b0-128">No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookChartSeries.](../resources/workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="415b0-128">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="415b0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="415b0-129">Response</span></span>

<span data-ttu-id="415b0-130">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [workbookChartSeries](../resources/workbookchartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="415b0-130">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="415b0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="415b0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="415b0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="415b0-132">Request</span></span>
<span data-ttu-id="415b0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="415b0-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="415b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="415b0-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="415b0-135">C#</span><span class="sxs-lookup"><span data-stu-id="415b0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="415b0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="415b0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="415b0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="415b0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="415b0-138">Java</span><span class="sxs-lookup"><span data-stu-id="415b0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartseries-from-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="415b0-139">No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookChartSeries.](../resources/workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="415b0-139">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="415b0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="415b0-140">Response</span></span>
<span data-ttu-id="415b0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="415b0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


