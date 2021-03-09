---
title: Create Chart
description: Use esta API para criar um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 306d538f06d2a1f2857f745580e9ab0e8cb9a59c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575116"
---
# <a name="create-chart"></a><span data-ttu-id="67b6b-103">Create Chart</span><span class="sxs-lookup"><span data-stu-id="67b6b-103">Create Chart</span></span>

<span data-ttu-id="67b6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67b6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67b6b-105">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="67b6b-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="67b6b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67b6b-106">Permissions</span></span>
<span data-ttu-id="67b6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67b6b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67b6b-109">Permission type</span></span>      | <span data-ttu-id="67b6b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67b6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67b6b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67b6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67b6b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67b6b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67b6b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67b6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67b6b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67b6b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67b6b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67b6b-115">Application</span></span> | <span data-ttu-id="67b6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67b6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67b6b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67b6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="67b6b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67b6b-118">Request headers</span></span>
| <span data-ttu-id="67b6b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="67b6b-119">Name</span></span>       | <span data-ttu-id="67b6b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="67b6b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67b6b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="67b6b-121">Authorization</span></span>  | <span data-ttu-id="67b6b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67b6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67b6b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="67b6b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="67b6b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="67b6b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67b6b-127">Request body</span></span>
<span data-ttu-id="67b6b-128">No corpo da solicitação, fornece uma representação JSON do [objeto workbookChart.](../resources/workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="67b6b-128">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="67b6b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b6b-129">Response</span></span>

<span data-ttu-id="67b6b-130">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67b6b-130">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67b6b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67b6b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67b6b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67b6b-132">Request</span></span>
<span data-ttu-id="67b6b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67b6b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67b6b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="67b6b-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67b6b-135">C#</span><span class="sxs-lookup"><span data-stu-id="67b6b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67b6b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67b6b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67b6b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67b6b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67b6b-138">Java</span><span class="sxs-lookup"><span data-stu-id="67b6b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="67b6b-139">No corpo da solicitação, fornece uma representação JSON do [objeto workbookChart.](../resources/workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="67b6b-139">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="67b6b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b6b-140">Response</span></span>
<span data-ttu-id="67b6b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67b6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


