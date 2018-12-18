---
title: Criar ChartSeries
description: Use essa API para criar novas ChartSeries.
author: lumine2008
ms.openlocfilehash: 727be89be598ff86d852a161f9888b286517f538
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304876"
---
# <a name="create-chartseries"></a><span data-ttu-id="12ec6-103">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="12ec6-103">Create ChartSeries</span></span>

<span data-ttu-id="12ec6-104">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="12ec6-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="12ec6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="12ec6-105">Permissions</span></span>
<span data-ttu-id="12ec6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12ec6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12ec6-108">Permission type</span></span>      | <span data-ttu-id="12ec6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12ec6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12ec6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12ec6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12ec6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12ec6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12ec6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12ec6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12ec6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12ec6-113">Not supported.</span></span>    |
|<span data-ttu-id="12ec6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12ec6-114">Application</span></span> | <span data-ttu-id="12ec6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12ec6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12ec6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12ec6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="12ec6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12ec6-117">Request headers</span></span>
| <span data-ttu-id="12ec6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="12ec6-118">Name</span></span>       | <span data-ttu-id="12ec6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ec6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12ec6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="12ec6-120">Authorization</span></span>  | <span data-ttu-id="12ec6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12ec6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12ec6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="12ec6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="12ec6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="12ec6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12ec6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12ec6-126">Request body</span></span>
<span data-ttu-id="12ec6-127">No corpo da solicitação, fornece uma representação JSON do objeto [WorkbookChartSeries](../resources/chartseries.md) .</span><span class="sxs-lookup"><span data-stu-id="12ec6-127">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12ec6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ec6-128">Response</span></span>

<span data-ttu-id="12ec6-129">Se tiver êxito, este método retornará `201 Created` código de resposta e o objeto [WorkbookChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12ec6-129">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12ec6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12ec6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12ec6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12ec6-131">Request</span></span>
<span data-ttu-id="12ec6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12ec6-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="12ec6-133">No corpo da solicitação, fornece uma representação JSON do objeto [WorkbookChartSeries](../resources/chartseries.md) .</span><span class="sxs-lookup"><span data-stu-id="12ec6-133">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="12ec6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ec6-134">Response</span></span>
<span data-ttu-id="12ec6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12ec6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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