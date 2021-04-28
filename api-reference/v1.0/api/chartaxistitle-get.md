---
title: Obter ChartAxisTitle
description: Recupera as propriedades e os relacionamentos do objeto chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 91d6694ac0e713391cf4c166ae10fea97d1b6adf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053276"
---
# <a name="get-chartaxistitle"></a><span data-ttu-id="e88b3-103">Obter ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="e88b3-103">Get ChartAxisTitle</span></span>

<span data-ttu-id="e88b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e88b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e88b3-105">Recupera as propriedades e os relacionamentos do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="e88b3-105">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e88b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e88b3-106">Permissions</span></span>
<span data-ttu-id="e88b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e88b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e88b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e88b3-109">Permission type</span></span>      | <span data-ttu-id="e88b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e88b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e88b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e88b3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e88b3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e88b3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e88b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e88b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e88b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e88b3-114">Not supported.</span></span>    |
|<span data-ttu-id="e88b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e88b3-115">Application</span></span> | <span data-ttu-id="e88b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e88b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e88b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e88b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e88b3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e88b3-118">Optional query parameters</span></span>
<span data-ttu-id="e88b3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e88b3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e88b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e88b3-120">Request headers</span></span>
| <span data-ttu-id="e88b3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e88b3-121">Name</span></span>      |<span data-ttu-id="e88b3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e88b3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e88b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e88b3-123">Authorization</span></span>  | <span data-ttu-id="e88b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e88b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e88b3-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e88b3-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e88b3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e88b3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e88b3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e88b3-129">Request body</span></span>
<span data-ttu-id="e88b3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e88b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e88b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e88b3-131">Response</span></span>

<span data-ttu-id="e88b3-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookChartAxisTitle](../resources/chartaxistitle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e88b3-132">If successful, this method returns a `200 OK` response code and [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e88b3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e88b3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e88b3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e88b3-134">Request</span></span>
<span data-ttu-id="e88b3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e88b3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e88b3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e88b3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
```
# <a name="c"></a>[<span data-ttu-id="e88b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="e88b3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e88b3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e88b3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e88b3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e88b3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e88b3-140">Java</span><span class="sxs-lookup"><span data-stu-id="e88b3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e88b3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e88b3-141">Response</span></span>
<span data-ttu-id="e88b3-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e88b3-142">Here is an example of the response.</span></span> <span data-ttu-id="e88b3-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e88b3-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
