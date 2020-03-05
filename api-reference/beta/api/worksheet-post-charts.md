---
title: Create Chart
description: Use esta API para criar um novo gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1ec6a1aa0d5d37e52924361f64e5e10291cf476b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451193"
---
# <a name="create-chart"></a><span data-ttu-id="bc7e4-103">Create Chart</span><span class="sxs-lookup"><span data-stu-id="bc7e4-103">Create Chart</span></span>

<span data-ttu-id="bc7e4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc7e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc7e4-105">Use esta API para criar um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc7e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc7e4-106">Permissions</span></span>
<span data-ttu-id="bc7e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc7e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc7e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc7e4-109">Permission type</span></span>      | <span data-ttu-id="bc7e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc7e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc7e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc7e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc7e4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc7e4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc7e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc7e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc7e4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc7e4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc7e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc7e4-115">Application</span></span> | <span data-ttu-id="bc7e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc7e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc7e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="bc7e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc7e4-118">Request headers</span></span>
| <span data-ttu-id="bc7e4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bc7e4-119">Name</span></span>       | <span data-ttu-id="bc7e4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc7e4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc7e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc7e4-121">Authorization</span></span>  | <span data-ttu-id="bc7e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc7e4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc7e4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc7e4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc7e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc7e4-127">Request body</span></span>
<span data-ttu-id="bc7e4-128">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChart](../resources/workbookchart.md) .</span><span class="sxs-lookup"><span data-stu-id="bc7e4-128">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bc7e4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc7e4-129">Response</span></span>

<span data-ttu-id="bc7e4-130">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbookChart](../resources/workbookchart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-130">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc7e4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc7e4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc7e4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc7e4-132">Request</span></span>
<span data-ttu-id="bc7e4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc7e4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc7e4-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bc7e4-135">C#</span><span class="sxs-lookup"><span data-stu-id="bc7e4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc7e4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc7e4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc7e4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc7e4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bc7e4-138">No corpo da solicitação, forneça uma representação JSON do objeto [workbookChart](../resources/workbookchart.md) .</span><span class="sxs-lookup"><span data-stu-id="bc7e4-138">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bc7e4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc7e4-139">Response</span></span>
<span data-ttu-id="bc7e4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc7e4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
