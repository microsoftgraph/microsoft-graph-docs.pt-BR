---
title: Obter ChartTitle
description: Recupera as propriedades e os relacionamentos do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 85de1cc95ef5a01eb490e1ea635380fa1474acc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316371"
---
# <a name="get-charttitle"></a><span data-ttu-id="87cfb-103">Obter ChartTitle</span><span class="sxs-lookup"><span data-stu-id="87cfb-103">Get ChartTitle</span></span>

<span data-ttu-id="87cfb-104">Recupera as propriedades e os relacionamentos do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="87cfb-104">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87cfb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="87cfb-105">Permissions</span></span>
<span data-ttu-id="87cfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87cfb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87cfb-108">Permission type</span></span>      | <span data-ttu-id="87cfb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87cfb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87cfb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87cfb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87cfb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87cfb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87cfb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87cfb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87cfb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87cfb-113">Not supported.</span></span>    |
|<span data-ttu-id="87cfb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87cfb-114">Application</span></span> | <span data-ttu-id="87cfb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87cfb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87cfb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87cfb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87cfb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87cfb-117">Optional query parameters</span></span>
<span data-ttu-id="87cfb-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87cfb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87cfb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87cfb-119">Request headers</span></span>
| <span data-ttu-id="87cfb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="87cfb-120">Name</span></span>      |<span data-ttu-id="87cfb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="87cfb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87cfb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87cfb-122">Authorization</span></span>  | <span data-ttu-id="87cfb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87cfb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87cfb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87cfb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="87cfb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="87cfb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87cfb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87cfb-128">Request body</span></span>
<span data-ttu-id="87cfb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87cfb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87cfb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87cfb-130">Response</span></span>

<span data-ttu-id="87cfb-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookChartTitle](../resources/charttitle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87cfb-131">If successful, this method returns a `200 OK` response code and [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87cfb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87cfb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87cfb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87cfb-133">Request</span></span>
<span data-ttu-id="87cfb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87cfb-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="87cfb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="87cfb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87cfb-136">C#</span><span class="sxs-lookup"><span data-stu-id="87cfb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87cfb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87cfb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87cfb-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="87cfb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="87cfb-139">Java</span><span class="sxs-lookup"><span data-stu-id="87cfb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87cfb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="87cfb-140">Response</span></span>
<span data-ttu-id="87cfb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87cfb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
