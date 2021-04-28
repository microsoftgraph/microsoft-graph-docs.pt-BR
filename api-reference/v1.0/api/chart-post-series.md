---
title: Criar ChartSeries
description: Use essa API para criar novas ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9468a415a02409a17862cec4486eee8156973e1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053283"
---
# <a name="create-chartseries"></a><span data-ttu-id="b7471-103">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b7471-103">Create ChartSeries</span></span>

<span data-ttu-id="b7471-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7471-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7471-105">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="b7471-105">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7471-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7471-106">Permissions</span></span>
<span data-ttu-id="b7471-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7471-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7471-109">Permission type</span></span>      | <span data-ttu-id="b7471-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7471-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7471-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7471-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7471-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7471-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7471-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7471-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7471-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7471-114">Not supported.</span></span>    |
|<span data-ttu-id="b7471-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7471-115">Application</span></span> | <span data-ttu-id="b7471-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7471-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7471-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7471-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="b7471-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7471-118">Request headers</span></span>
| <span data-ttu-id="b7471-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b7471-119">Name</span></span>       | <span data-ttu-id="b7471-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7471-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7471-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7471-121">Authorization</span></span>  | <span data-ttu-id="b7471-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7471-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7471-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7471-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7471-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b7471-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7471-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7471-127">Request body</span></span>
<span data-ttu-id="b7471-128">No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookChartSeries.](../resources/chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="b7471-128">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b7471-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7471-129">Response</span></span>

<span data-ttu-id="b7471-130">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto WorkbookChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7471-130">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7471-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7471-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7471-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7471-132">Request</span></span>
<span data-ttu-id="b7471-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7471-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7471-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7471-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b7471-135">C#</span><span class="sxs-lookup"><span data-stu-id="b7471-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7471-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7471-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7471-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7471-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7471-138">Java</span><span class="sxs-lookup"><span data-stu-id="b7471-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartseries-from-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b7471-139">No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookChartSeries.](../resources/chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="b7471-139">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b7471-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7471-140">Response</span></span>
<span data-ttu-id="b7471-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7471-141">Here is an example of the response.</span></span> <span data-ttu-id="b7471-142">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b7471-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

