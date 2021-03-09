---
title: Listar ChartPointsCollection
description: Recupera uma lista de objetos chartpoint.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 66383d9c02f296ad268d80f4cebb40fa717e0ae2
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574444"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="b803a-103">Listar ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="b803a-103">List ChartPointsCollection</span></span>

<span data-ttu-id="b803a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b803a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b803a-105">Recupera uma lista de objetos chartpoint.</span><span class="sxs-lookup"><span data-stu-id="b803a-105">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b803a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b803a-106">Permissions</span></span>
<span data-ttu-id="b803a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b803a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b803a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b803a-109">Permission type</span></span>      | <span data-ttu-id="b803a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b803a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b803a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b803a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b803a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b803a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b803a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b803a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b803a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b803a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b803a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b803a-115">Application</span></span> | <span data-ttu-id="b803a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b803a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b803a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b803a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b803a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b803a-118">Optional query parameters</span></span>
<span data-ttu-id="b803a-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b803a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b803a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b803a-120">Request headers</span></span>
| <span data-ttu-id="b803a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b803a-121">Name</span></span>      |<span data-ttu-id="b803a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b803a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b803a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b803a-123">Authorization</span></span>  | <span data-ttu-id="b803a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b803a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b803a-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b803a-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b803a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b803a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b803a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b803a-129">Request body</span></span>
<span data-ttu-id="b803a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b803a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b803a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b803a-131">Response</span></span>

<span data-ttu-id="b803a-132">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b803a-132">If successful, this method returns a `200 OK` response code and collection of [workbookChartPoint](../resources/workbookchartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b803a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b803a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b803a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b803a-134">Request</span></span>
<span data-ttu-id="b803a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b803a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b803a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b803a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
```
# <a name="c"></a>[<span data-ttu-id="b803a-137">C#</span><span class="sxs-lookup"><span data-stu-id="b803a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartpointscollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b803a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b803a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartpointscollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b803a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b803a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartpointscollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b803a-140">Java</span><span class="sxs-lookup"><span data-stu-id="b803a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartpointscollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b803a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b803a-141">Response</span></span>
<span data-ttu-id="b803a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b803a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
