---
title: Create Chart
description: Use esta API para criar um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 82d129e5b52e1e17ffb09f037ad8b819a8c7a708
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456516"
---
# <a name="create-chart"></a><span data-ttu-id="df9e2-103">Create Chart</span><span class="sxs-lookup"><span data-stu-id="df9e2-103">Create Chart</span></span>

<span data-ttu-id="df9e2-104">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="df9e2-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="df9e2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="df9e2-105">Permissions</span></span>
<span data-ttu-id="df9e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df9e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df9e2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df9e2-108">Permission type</span></span>      | <span data-ttu-id="df9e2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df9e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df9e2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df9e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="df9e2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df9e2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df9e2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df9e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df9e2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df9e2-113">Not supported.</span></span>    |
|<span data-ttu-id="df9e2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df9e2-114">Application</span></span> | <span data-ttu-id="df9e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df9e2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df9e2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df9e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="df9e2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df9e2-117">Request headers</span></span>
| <span data-ttu-id="df9e2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="df9e2-118">Name</span></span>       | <span data-ttu-id="df9e2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="df9e2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df9e2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="df9e2-120">Authorization</span></span>  | <span data-ttu-id="df9e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df9e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df9e2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="df9e2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="df9e2-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="df9e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df9e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df9e2-126">Request body</span></span>
<span data-ttu-id="df9e2-127">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookChart](../resources/chart.md) .</span><span class="sxs-lookup"><span data-stu-id="df9e2-127">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df9e2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df9e2-128">Response</span></span>

<span data-ttu-id="df9e2-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df9e2-129">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df9e2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df9e2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df9e2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df9e2-131">Request</span></span>
<span data-ttu-id="df9e2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df9e2-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df9e2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df9e2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df9e2-134">C#</span><span class="sxs-lookup"><span data-stu-id="df9e2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df9e2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="df9e2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df9e2-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="df9e2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="df9e2-137">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookChart](../resources/chart.md) .</span><span class="sxs-lookup"><span data-stu-id="df9e2-137">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="df9e2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="df9e2-138">Response</span></span>
<span data-ttu-id="df9e2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df9e2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
