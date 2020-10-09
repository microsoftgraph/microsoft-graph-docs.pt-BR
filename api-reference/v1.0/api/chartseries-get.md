---
title: Obter ChartSeries
description: Recupera as propriedades e os relacionamentos do objeto chartseries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: eeca570f11264acaeea85586ae2d83ec315e09f4
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401332"
---
# <a name="get-chartseries"></a><span data-ttu-id="c0e53-103">Obter ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c0e53-103">Get ChartSeries</span></span>

<span data-ttu-id="c0e53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0e53-105">Recupera as propriedades e os relacionamentos do objeto chartseries.</span><span class="sxs-lookup"><span data-stu-id="c0e53-105">Retrieve the properties and relationships of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0e53-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0e53-106">Permissions</span></span>
<span data-ttu-id="c0e53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0e53-109">Permission type</span></span>      | <span data-ttu-id="c0e53-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0e53-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0e53-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0e53-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0e53-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0e53-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0e53-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0e53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0e53-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0e53-114">Not supported.</span></span>    |
|<span data-ttu-id="c0e53-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0e53-115">Application</span></span> | <span data-ttu-id="c0e53-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0e53-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0e53-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0e53-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0e53-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0e53-118">Optional query parameters</span></span>
<span data-ttu-id="c0e53-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e53-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0e53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e53-120">Request headers</span></span>
| <span data-ttu-id="c0e53-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c0e53-121">Name</span></span>      |<span data-ttu-id="c0e53-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0e53-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0e53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0e53-123">Authorization</span></span>  | <span data-ttu-id="c0e53-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0e53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0e53-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0e53-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0e53-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0e53-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e53-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e53-129">Request body</span></span>
<span data-ttu-id="c0e53-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0e53-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e53-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0e53-131">Response</span></span>

<span data-ttu-id="c0e53-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e53-132">If successful, this method returns a `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0e53-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0e53-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0e53-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e53-134">Request</span></span>
<span data-ttu-id="c0e53-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0e53-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0e53-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0e53-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartseries"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
# <a name="c"></a>[<span data-ttu-id="c0e53-137">C#</span><span class="sxs-lookup"><span data-stu-id="c0e53-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0e53-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0e53-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0e53-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0e53-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0e53-140">Java</span><span class="sxs-lookup"><span data-stu-id="c0e53-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0e53-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0e53-141">Response</span></span>
<span data-ttu-id="c0e53-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0e53-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->