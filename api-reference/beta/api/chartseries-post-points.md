---
title: Criar ChartPoints
description: Use essa API para criar novos ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 057f8be5fa646cef0a5d39fe758e8901b9e4c583
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316733"
---
# <a name="create-chartpoint"></a><span data-ttu-id="582e1-103">Criar ChartPoint</span><span class="sxs-lookup"><span data-stu-id="582e1-103">Create ChartPoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="582e1-104">Use esta API para criar um novo ChartPoint.</span><span class="sxs-lookup"><span data-stu-id="582e1-104">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="582e1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="582e1-105">Permissions</span></span>
<span data-ttu-id="582e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="582e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="582e1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="582e1-108">Permission type</span></span>      | <span data-ttu-id="582e1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="582e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="582e1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="582e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="582e1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="582e1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="582e1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="582e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="582e1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="582e1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="582e1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="582e1-114">Application</span></span> | <span data-ttu-id="582e1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="582e1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="582e1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="582e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="582e1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="582e1-117">Request headers</span></span>
| <span data-ttu-id="582e1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="582e1-118">Name</span></span>       | <span data-ttu-id="582e1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="582e1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="582e1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="582e1-120">Authorization</span></span>  | <span data-ttu-id="582e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="582e1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="582e1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="582e1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="582e1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="582e1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="582e1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="582e1-126">Request body</span></span>
<span data-ttu-id="582e1-127">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChartPoint](../resources/workbookchartpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="582e1-127">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="582e1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="582e1-128">Response</span></span>

<span data-ttu-id="582e1-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="582e1-129">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="582e1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="582e1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="582e1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="582e1-131">Request</span></span>
<span data-ttu-id="582e1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="582e1-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="582e1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="582e1-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="582e1-134">C#</span><span class="sxs-lookup"><span data-stu-id="582e1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="582e1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="582e1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="582e1-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="582e1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="582e1-137">Java</span><span class="sxs-lookup"><span data-stu-id="582e1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="582e1-138">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChartPoint](../resources/workbookchartpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="582e1-138">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="582e1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="582e1-139">Response</span></span>
<span data-ttu-id="582e1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="582e1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
