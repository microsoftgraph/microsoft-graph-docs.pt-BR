---
title: Criar ChartSeries
description: Use essa API para criar novas ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 053fd380728928241c146787c03b87a5207a0b7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927531"
---
# <a name="create-chartseries"></a><span data-ttu-id="f22b4-103">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="f22b4-103">Create ChartSeries</span></span>

<span data-ttu-id="f22b4-104">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="f22b4-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="f22b4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f22b4-105">Permissions</span></span>
<span data-ttu-id="f22b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f22b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f22b4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f22b4-108">Permission type</span></span>      | <span data-ttu-id="f22b4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f22b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f22b4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f22b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f22b4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f22b4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f22b4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f22b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f22b4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f22b4-113">Not supported.</span></span>    |
|<span data-ttu-id="f22b4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f22b4-114">Application</span></span> | <span data-ttu-id="f22b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f22b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f22b4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f22b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="f22b4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f22b4-117">Request headers</span></span>
| <span data-ttu-id="f22b4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f22b4-118">Name</span></span>       | <span data-ttu-id="f22b4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f22b4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f22b4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f22b4-120">Authorization</span></span>  | <span data-ttu-id="f22b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f22b4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f22b4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f22b4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f22b4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f22b4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f22b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f22b4-126">Request body</span></span>
<span data-ttu-id="f22b4-127">No corpo da solicitação, fornece uma representação JSON do objeto [WorkbookChartSeries](../resources/chartseries.md) .</span><span class="sxs-lookup"><span data-stu-id="f22b4-127">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f22b4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22b4-128">Response</span></span>

<span data-ttu-id="f22b4-129">Se tiver êxito, este método retornará `201 Created` código de resposta e o objeto [WorkbookChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f22b4-129">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f22b4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f22b4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f22b4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f22b4-131">Request</span></span>
<span data-ttu-id="f22b4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f22b4-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="f22b4-133">No corpo da solicitação, fornece uma representação JSON do objeto [WorkbookChartSeries](../resources/chartseries.md) .</span><span class="sxs-lookup"><span data-stu-id="f22b4-133">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f22b4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22b4-134">Response</span></span>
<span data-ttu-id="f22b4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f22b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
