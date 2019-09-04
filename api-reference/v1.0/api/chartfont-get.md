---
title: Obter ChartFont
description: Recupera as propriedades e os relacionamentos do objeto chartfont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f1e4185ed1d771a0049c454431fc48bfc90a9850
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727275"
---
# <a name="get-chartfont"></a><span data-ttu-id="ba140-103">Obter ChartFont</span><span class="sxs-lookup"><span data-stu-id="ba140-103">Get ChartFont</span></span>

<span data-ttu-id="ba140-104">Recupera as propriedades e os relacionamentos do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="ba140-104">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba140-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba140-105">Permissions</span></span>
<span data-ttu-id="ba140-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba140-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba140-108">Permission type</span></span>      | <span data-ttu-id="ba140-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba140-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba140-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba140-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba140-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba140-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ba140-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba140-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba140-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba140-113">Not supported.</span></span>    |
|<span data-ttu-id="ba140-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba140-114">Application</span></span> | <span data-ttu-id="ba140-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba140-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba140-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba140-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba140-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba140-117">Optional query parameters</span></span>
<span data-ttu-id="ba140-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba140-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba140-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba140-119">Request headers</span></span>
| <span data-ttu-id="ba140-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ba140-120">Name</span></span>      |<span data-ttu-id="ba140-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba140-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba140-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba140-122">Authorization</span></span>  | <span data-ttu-id="ba140-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba140-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba140-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ba140-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ba140-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ba140-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba140-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba140-128">Request body</span></span>
<span data-ttu-id="ba140-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba140-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba140-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba140-130">Response</span></span>

<span data-ttu-id="ba140-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartFont](../resources/chartfont.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba140-131">If successful, this method returns a `200 OK` response code and [WorkbookChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba140-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba140-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba140-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba140-133">Request</span></span>
<span data-ttu-id="ba140-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba140-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba140-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba140-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba140-136">C#</span><span class="sxs-lookup"><span data-stu-id="ba140-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba140-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba140-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba140-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ba140-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ba140-139">Java</span><span class="sxs-lookup"><span data-stu-id="ba140-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ba140-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba140-140">Response</span></span>
<span data-ttu-id="ba140-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba140-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
