---
title: Criar ChartPoints
description: Use essa API para criar novos ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3c9a98f731b58a55b70a27b0d39fd6d0d2b2d240
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574360"
---
# <a name="create-chartpoint"></a><span data-ttu-id="127e3-103">Criar ChartPoint</span><span class="sxs-lookup"><span data-stu-id="127e3-103">Create ChartPoint</span></span>

<span data-ttu-id="127e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="127e3-105">Use essa API para criar um novo ChartPoint.</span><span class="sxs-lookup"><span data-stu-id="127e3-105">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="127e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="127e3-106">Permissions</span></span>
<span data-ttu-id="127e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="127e3-109">Permission type</span></span>      | <span data-ttu-id="127e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="127e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="127e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="127e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="127e3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127e3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="127e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="127e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="127e3-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="127e3-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="127e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="127e3-115">Application</span></span> | <span data-ttu-id="127e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="127e3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="127e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="127e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="127e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="127e3-118">Request headers</span></span>
| <span data-ttu-id="127e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="127e3-119">Name</span></span>       | <span data-ttu-id="127e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="127e3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="127e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="127e3-121">Authorization</span></span>  | <span data-ttu-id="127e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="127e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="127e3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="127e3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="127e3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="127e3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="127e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="127e3-127">Request body</span></span>
<span data-ttu-id="127e3-128">No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookChartPoint.](../resources/workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="127e3-128">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="127e3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="127e3-129">Response</span></span>

<span data-ttu-id="127e3-130">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="127e3-130">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="127e3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="127e3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="127e3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="127e3-132">Request</span></span>
<span data-ttu-id="127e3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="127e3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="127e3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="127e3-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="127e3-135">C#</span><span class="sxs-lookup"><span data-stu-id="127e3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="127e3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="127e3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="127e3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="127e3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="127e3-138">Java</span><span class="sxs-lookup"><span data-stu-id="127e3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="127e3-139">No corpo da solicitação, fornece uma representação JSON do [objeto WorkbookChartPoint.](../resources/workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="127e3-139">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="127e3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="127e3-140">Response</span></span>
<span data-ttu-id="127e3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="127e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->


