---
title: Obter ChartDataLabels
description: Lê as propriedades e os relacionamentos do objeto chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0b0877780db5954ed729b1ec461bbde265b8a96b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331956"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="465b1-103">Obter ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="465b1-103">Get ChartDataLabels</span></span>

<span data-ttu-id="465b1-104">Lê as propriedades e os relacionamentos do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="465b1-104">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="465b1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="465b1-105">Permissions</span></span>
<span data-ttu-id="465b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="465b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="465b1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="465b1-108">Permission type</span></span>      | <span data-ttu-id="465b1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="465b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="465b1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="465b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="465b1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="465b1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="465b1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="465b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="465b1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="465b1-113">Not supported.</span></span>    |
|<span data-ttu-id="465b1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="465b1-114">Application</span></span> | <span data-ttu-id="465b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="465b1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="465b1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="465b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="465b1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="465b1-117">Optional query parameters</span></span>
<span data-ttu-id="465b1-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="465b1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="465b1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="465b1-119">Request headers</span></span>
| <span data-ttu-id="465b1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="465b1-120">Name</span></span>      |<span data-ttu-id="465b1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="465b1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="465b1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="465b1-122">Authorization</span></span>  | <span data-ttu-id="465b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="465b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="465b1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="465b1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="465b1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="465b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="465b1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="465b1-128">Request body</span></span>
<span data-ttu-id="465b1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="465b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="465b1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="465b1-130">Response</span></span>

<span data-ttu-id="465b1-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartDataLabels](../resources/chartdatalabels.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="465b1-131">If successful, this method returns a `200 OK` response code and [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="465b1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="465b1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="465b1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="465b1-133">Request</span></span>
<span data-ttu-id="465b1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="465b1-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="465b1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="465b1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="465b1-136">C#</span><span class="sxs-lookup"><span data-stu-id="465b1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="465b1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="465b1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="465b1-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="465b1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="465b1-139">Java</span><span class="sxs-lookup"><span data-stu-id="465b1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="465b1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="465b1-140">Response</span></span>
<span data-ttu-id="465b1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="465b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
