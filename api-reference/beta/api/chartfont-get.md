---
title: Obter workbookChartFont
description: Recupere as propriedades e os relacionamentos do objeto workbookChartFont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7aecb07f8120ae5383df288e8d282e1c2ba40742
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371936"
---
# <a name="get-workbookchartfont"></a><span data-ttu-id="34fb8-103">Obter workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="34fb8-103">Get workbookChartFont</span></span>

<span data-ttu-id="34fb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34fb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34fb8-105">Recupera as propriedades e os relacionamentos do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="34fb8-105">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34fb8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34fb8-106">Permissions</span></span>
<span data-ttu-id="34fb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34fb8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34fb8-109">Permission type</span></span>      | <span data-ttu-id="34fb8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34fb8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34fb8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34fb8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34fb8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34fb8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34fb8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34fb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34fb8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34fb8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34fb8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34fb8-115">Application</span></span> | <span data-ttu-id="34fb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34fb8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34fb8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34fb8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34fb8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34fb8-118">Optional query parameters</span></span>
<span data-ttu-id="34fb8-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34fb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34fb8-120">Request headers</span></span>
| <span data-ttu-id="34fb8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="34fb8-121">Name</span></span>      |<span data-ttu-id="34fb8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="34fb8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34fb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34fb8-123">Authorization</span></span>  | <span data-ttu-id="34fb8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34fb8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34fb8-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34fb8-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="34fb8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="34fb8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34fb8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34fb8-129">Request body</span></span>
<span data-ttu-id="34fb8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34fb8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34fb8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="34fb8-131">Response</span></span>

<span data-ttu-id="34fb8-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartFont](../resources/workbookchartfont.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34fb8-132">If successful, this method returns a `200 OK` response code and [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34fb8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34fb8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34fb8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34fb8-134">Request</span></span>
<span data-ttu-id="34fb8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34fb8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34fb8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="34fb8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
```
# <a name="c"></a>[<span data-ttu-id="34fb8-137">C#</span><span class="sxs-lookup"><span data-stu-id="34fb8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34fb8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34fb8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34fb8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34fb8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="34fb8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="34fb8-140">Response</span></span>
<span data-ttu-id="34fb8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34fb8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
