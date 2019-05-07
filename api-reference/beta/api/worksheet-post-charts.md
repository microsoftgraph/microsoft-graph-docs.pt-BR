---
title: Create Chart
description: Use esta API para criar um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a7b16048f889913c8721c29479131d2b6caa04a9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636846"
---
# <a name="create-chart"></a><span data-ttu-id="85377-103">Create Chart</span><span class="sxs-lookup"><span data-stu-id="85377-103">Create Chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85377-104">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="85377-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="85377-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85377-105">Permissions</span></span>
<span data-ttu-id="85377-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85377-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85377-108">Permission type</span></span>      | <span data-ttu-id="85377-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85377-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85377-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85377-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85377-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85377-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85377-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85377-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85377-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85377-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85377-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85377-114">Application</span></span> | <span data-ttu-id="85377-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85377-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85377-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85377-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="85377-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85377-117">Request headers</span></span>
| <span data-ttu-id="85377-118">Nome</span><span class="sxs-lookup"><span data-stu-id="85377-118">Name</span></span>       | <span data-ttu-id="85377-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="85377-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="85377-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="85377-120">Authorization</span></span>  | <span data-ttu-id="85377-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85377-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85377-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85377-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="85377-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="85377-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85377-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85377-126">Request body</span></span>
<span data-ttu-id="85377-127">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChart](../resources/workbookchart.md) .</span><span class="sxs-lookup"><span data-stu-id="85377-127">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="85377-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="85377-128">Response</span></span>

<span data-ttu-id="85377-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85377-129">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85377-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85377-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85377-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85377-131">Request</span></span>
<span data-ttu-id="85377-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85377-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="85377-133">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChart](../resources/workbookchart.md) .</span><span class="sxs-lookup"><span data-stu-id="85377-133">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="85377-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85377-134">Response</span></span>
<span data-ttu-id="85377-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85377-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="85377-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="85377-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85377-139">Basic</span><span class="sxs-lookup"><span data-stu-id="85377-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chart_from_worksheet-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85377-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85377-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chart_from_worksheet-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-post-charts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheet-post-charts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
