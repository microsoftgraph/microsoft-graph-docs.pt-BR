---
title: Create Chart
description: Use esta API para criar um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5101a83c67f7c28d9859db27055db6e752748404
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051631"
---
# <a name="create-chart"></a><span data-ttu-id="fdffb-103">Create Chart</span><span class="sxs-lookup"><span data-stu-id="fdffb-103">Create Chart</span></span>

<span data-ttu-id="fdffb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdffb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdffb-105">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="fdffb-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdffb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdffb-106">Permissions</span></span>
<span data-ttu-id="fdffb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdffb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdffb-109">Permission type</span></span>      | <span data-ttu-id="fdffb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdffb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdffb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdffb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fdffb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdffb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fdffb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdffb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdffb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdffb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fdffb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdffb-115">Application</span></span> | <span data-ttu-id="fdffb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdffb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdffb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdffb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="fdffb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdffb-118">Request headers</span></span>
| <span data-ttu-id="fdffb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fdffb-119">Name</span></span>       | <span data-ttu-id="fdffb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdffb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fdffb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdffb-121">Authorization</span></span>  | <span data-ttu-id="fdffb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdffb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fdffb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fdffb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fdffb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fdffb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdffb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdffb-127">Request body</span></span>
<span data-ttu-id="fdffb-128">No corpo da solicitação, fornece uma representação JSON do [objeto workbookChart.](../resources/workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="fdffb-128">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fdffb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdffb-129">Response</span></span>

<span data-ttu-id="fdffb-130">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdffb-130">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdffb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdffb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdffb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdffb-132">Request</span></span>
<span data-ttu-id="fdffb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdffb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fdffb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdffb-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fdffb-135">C#</span><span class="sxs-lookup"><span data-stu-id="fdffb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdffb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdffb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdffb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdffb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdffb-138">Java</span><span class="sxs-lookup"><span data-stu-id="fdffb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fdffb-139">No corpo da solicitação, fornece uma representação JSON do [objeto workbookChart.](../resources/workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="fdffb-139">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fdffb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdffb-140">Response</span></span>
<span data-ttu-id="fdffb-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdffb-141">Here is an example of the response.</span></span> <span data-ttu-id="fdffb-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fdffb-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


