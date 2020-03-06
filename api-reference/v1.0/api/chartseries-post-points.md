---
title: Criar ChartPoints
description: Use essa API para criar novos ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fa377fe309404d4a18be91a30e97cc5bec49cc8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518347"
---
# <a name="create-chartpoints"></a><span data-ttu-id="1cc37-103">Criar ChartPoints</span><span class="sxs-lookup"><span data-stu-id="1cc37-103">Create ChartPoints</span></span>

<span data-ttu-id="1cc37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cc37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1cc37-105">Use essa API para criar novos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="1cc37-105">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="1cc37-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cc37-106">Permissions</span></span>
<span data-ttu-id="1cc37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cc37-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc37-109">Permission type</span></span>      | <span data-ttu-id="1cc37-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc37-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc37-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc37-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc37-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cc37-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1cc37-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc37-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc37-114">Not supported.</span></span>    |
|<span data-ttu-id="1cc37-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc37-115">Application</span></span> | <span data-ttu-id="1cc37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc37-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc37-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc37-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points

```
## <a name="request-headers"></a><span data-ttu-id="1cc37-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc37-118">Request headers</span></span>
| <span data-ttu-id="1cc37-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1cc37-119">Name</span></span>       | <span data-ttu-id="1cc37-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc37-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1cc37-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cc37-121">Authorization</span></span>  | <span data-ttu-id="1cc37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cc37-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1cc37-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1cc37-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1cc37-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cc37-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cc37-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc37-127">Request body</span></span>
<span data-ttu-id="1cc37-128">No corpo da solicitação, forneça uma representação JSON do objeto [ChartPoints](../resources/chartpoint.md).</span><span class="sxs-lookup"><span data-stu-id="1cc37-128">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1cc37-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc37-129">Response</span></span>

<span data-ttu-id="1cc37-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ChartPoints](../resources/chartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc37-130">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cc37-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cc37-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cc37-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc37-132">Request</span></span>
<span data-ttu-id="1cc37-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc37-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cc37-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc37-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
Content-type: application/json
Content-length: 3

{
}
```
# <a name="c"></a>[<span data-ttu-id="1cc37-135">C#</span><span class="sxs-lookup"><span data-stu-id="1cc37-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cc37-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cc37-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cc37-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cc37-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cc37-138">Java</span><span class="sxs-lookup"><span data-stu-id="1cc37-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1cc37-139">No corpo da solicitação, forneça uma representação JSON do objeto [ChartPoints](../resources/chartpoint.md).</span><span class="sxs-lookup"><span data-stu-id="1cc37-139">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1cc37-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc37-140">Response</span></span>
<span data-ttu-id="1cc37-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cc37-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
