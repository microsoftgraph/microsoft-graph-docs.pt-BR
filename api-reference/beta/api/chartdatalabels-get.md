---
title: Obter workbookChartDataLabels
description: Recupere as propriedades e os relacionamentos do objeto workbookchartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: db36f45365375bd51c6701a4ac632d0c0afffa13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439510"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="9a1d8-103">Obter ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="9a1d8-103">Get ChartDataLabels</span></span>

<span data-ttu-id="9a1d8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9a1d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a1d8-105">Lê as propriedades e os relacionamentos do objeto chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-105">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a1d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a1d8-106">Permissions</span></span>
<span data-ttu-id="9a1d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a1d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a1d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a1d8-109">Permission type</span></span>      | <span data-ttu-id="9a1d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a1d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a1d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a1d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a1d8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a1d8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a1d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a1d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a1d8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a1d8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a1d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a1d8-115">Application</span></span> | <span data-ttu-id="9a1d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a1d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a1d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a1d8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a1d8-118">Optional query parameters</span></span>
<span data-ttu-id="9a1d8-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a1d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a1d8-120">Request headers</span></span>
| <span data-ttu-id="9a1d8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9a1d8-121">Name</span></span>      |<span data-ttu-id="9a1d8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a1d8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a1d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a1d8-123">Authorization</span></span>  | <span data-ttu-id="9a1d8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a1d8-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a1d8-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a1d8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a1d8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a1d8-129">Request body</span></span>
<span data-ttu-id="9a1d8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a1d8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a1d8-131">Response</span></span>

<span data-ttu-id="9a1d8-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartDataLabels](../resources/workbookchartdatalabels.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-132">If successful, this method returns a `200 OK` response code and [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a1d8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a1d8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a1d8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a1d8-134">Request</span></span>
<span data-ttu-id="9a1d8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a1d8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a1d8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
```
# <a name="c"></a>[<span data-ttu-id="9a1d8-137">C#</span><span class="sxs-lookup"><span data-stu-id="9a1d8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a1d8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a1d8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a1d8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a1d8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a1d8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a1d8-140">Response</span></span>
<span data-ttu-id="9a1d8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a1d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
