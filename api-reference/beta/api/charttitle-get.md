---
title: Obter ChartTitle
description: Recupera as propriedades e os relacionamentos do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d9ed64f86a250becac0a7b349c81800b547372d2
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574332"
---
# <a name="get-charttitle"></a><span data-ttu-id="50672-103">Obter ChartTitle</span><span class="sxs-lookup"><span data-stu-id="50672-103">Get ChartTitle</span></span>

<span data-ttu-id="50672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50672-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50672-105">Recupera as propriedades e os relacionamentos do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="50672-105">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="50672-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50672-106">Permissions</span></span>
<span data-ttu-id="50672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50672-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50672-109">Permission type</span></span>      | <span data-ttu-id="50672-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50672-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50672-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50672-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50672-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50672-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50672-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50672-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50672-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50672-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50672-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50672-115">Application</span></span> | <span data-ttu-id="50672-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50672-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50672-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50672-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50672-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50672-118">Optional query parameters</span></span>
<span data-ttu-id="50672-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50672-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50672-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50672-120">Request headers</span></span>
| <span data-ttu-id="50672-121">Nome</span><span class="sxs-lookup"><span data-stu-id="50672-121">Name</span></span>      |<span data-ttu-id="50672-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="50672-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50672-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="50672-123">Authorization</span></span>  | <span data-ttu-id="50672-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50672-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50672-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="50672-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="50672-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="50672-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50672-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50672-129">Request body</span></span>
<span data-ttu-id="50672-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50672-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50672-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="50672-131">Response</span></span>

<span data-ttu-id="50672-132">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [workbookChartTitle](../resources/workbookcharttitle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50672-132">If successful, this method returns a `200 OK` response code and [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50672-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50672-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50672-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50672-134">Request</span></span>
<span data-ttu-id="50672-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50672-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50672-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="50672-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
# <a name="c"></a>[<span data-ttu-id="50672-137">C#</span><span class="sxs-lookup"><span data-stu-id="50672-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50672-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50672-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50672-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50672-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50672-140">Java</span><span class="sxs-lookup"><span data-stu-id="50672-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50672-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="50672-141">Response</span></span>
<span data-ttu-id="50672-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50672-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
