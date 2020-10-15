---
title: Obter ChartGridlines
description: Recupera as propriedades e os relacionamentos do objeto chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cd0597f925899a0fde0bb94077fec45f6e43e0b7
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459400"
---
# <a name="get-chartgridlines"></a><span data-ttu-id="d3897-103">Obter ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="d3897-103">Get ChartGridlines</span></span>

<span data-ttu-id="d3897-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3897-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3897-105">Recupera as propriedades e os relacionamentos do objeto chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="d3897-105">Retrieve the properties and relationships of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3897-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d3897-106">Permissions</span></span>
<span data-ttu-id="d3897-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3897-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3897-109">Permission type</span></span>      | <span data-ttu-id="d3897-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3897-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3897-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3897-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3897-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3897-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3897-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3897-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3897-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3897-114">Not supported.</span></span>    |
|<span data-ttu-id="d3897-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3897-115">Application</span></span> | <span data-ttu-id="d3897-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3897-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3897-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3897-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3897-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3897-118">Optional query parameters</span></span>
<span data-ttu-id="d3897-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3897-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3897-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3897-120">Request headers</span></span>
| <span data-ttu-id="d3897-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d3897-121">Name</span></span>      |<span data-ttu-id="d3897-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3897-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3897-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3897-123">Authorization</span></span>  | <span data-ttu-id="d3897-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3897-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3897-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3897-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3897-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3897-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3897-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3897-129">Request body</span></span>
<span data-ttu-id="d3897-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3897-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3897-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3897-131">Response</span></span>

<span data-ttu-id="d3897-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartGridlines](../resources/chartgridlines.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3897-132">If successful, this method returns a `200 OK` response code and [WorkbookChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3897-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3897-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3897-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3897-134">Request</span></span>
<span data-ttu-id="d3897-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3897-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3897-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3897-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartgridlines"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
```
# <a name="c"></a>[<span data-ttu-id="d3897-137">C#</span><span class="sxs-lookup"><span data-stu-id="d3897-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3897-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3897-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3897-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3897-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3897-140">Java</span><span class="sxs-lookup"><span data-stu-id="d3897-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartgridlines-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3897-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3897-141">Response</span></span>
<span data-ttu-id="d3897-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3897-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartGridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
