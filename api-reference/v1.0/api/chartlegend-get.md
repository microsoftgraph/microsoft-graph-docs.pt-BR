---
title: Obter ChartLegend
description: Recupera as propriedades e os relacionamentos do objeto chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 56c049f0f0b4c90ca7fecb9f6d6262b1c6b81813
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003494"
---
# <a name="get-chartlegend"></a><span data-ttu-id="9a05c-103">Obter ChartLegend</span><span class="sxs-lookup"><span data-stu-id="9a05c-103">Get ChartLegend</span></span>

<span data-ttu-id="9a05c-104">Recupera as propriedades e os relacionamentos do objeto chartlegend.</span><span class="sxs-lookup"><span data-stu-id="9a05c-104">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a05c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a05c-105">Permissions</span></span>
<span data-ttu-id="9a05c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a05c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a05c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a05c-108">Permission type</span></span>      | <span data-ttu-id="9a05c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a05c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a05c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a05c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a05c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a05c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a05c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a05c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a05c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a05c-113">Not supported.</span></span>    |
|<span data-ttu-id="9a05c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a05c-114">Application</span></span> | <span data-ttu-id="9a05c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a05c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a05c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a05c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a05c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a05c-117">Optional query parameters</span></span>
<span data-ttu-id="9a05c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a05c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a05c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a05c-119">Request headers</span></span>
| <span data-ttu-id="9a05c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9a05c-120">Name</span></span>      |<span data-ttu-id="9a05c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a05c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a05c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a05c-122">Authorization</span></span>  | <span data-ttu-id="9a05c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a05c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a05c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a05c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a05c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a05c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a05c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a05c-128">Request body</span></span>
<span data-ttu-id="9a05c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a05c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a05c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a05c-130">Response</span></span>

<span data-ttu-id="9a05c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartLegend](../resources/chartlegend.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a05c-131">If successful, this method returns a `200 OK` response code and [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a05c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a05c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a05c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a05c-133">Request</span></span>
<span data-ttu-id="9a05c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a05c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a05c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a05c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a05c-136">C#</span><span class="sxs-lookup"><span data-stu-id="9a05c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a05c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a05c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a05c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9a05c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a05c-139">Java</span><span class="sxs-lookup"><span data-stu-id="9a05c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a05c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a05c-140">Response</span></span>
<span data-ttu-id="9a05c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a05c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartLegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
