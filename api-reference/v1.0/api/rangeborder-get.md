---
title: Obter RangeBorder
description: Recupere as propriedades e os relacionamentos do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 793b629947c61429d9bf936b5990a94f8b2eda26
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607906"
---
# <a name="get-rangeborder"></a><span data-ttu-id="dcb28-103">Obter RangeBorder</span><span class="sxs-lookup"><span data-stu-id="dcb28-103">Get RangeBorder</span></span>

<span data-ttu-id="dcb28-104">Recupere as propriedades e os relacionamentos do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="dcb28-104">Retrieve the properties and relationships of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dcb28-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcb28-105">Permissions</span></span>
<span data-ttu-id="dcb28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcb28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcb28-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcb28-108">Permission type</span></span>      | <span data-ttu-id="dcb28-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcb28-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcb28-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcb28-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcb28-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcb28-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dcb28-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcb28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcb28-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcb28-113">Not supported.</span></span>    |
|<span data-ttu-id="dcb28-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcb28-114">Application</span></span> | <span data-ttu-id="dcb28-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcb28-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcb28-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcb28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders/{sideIndex}
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dcb28-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dcb28-117">Optional query parameters</span></span>
<span data-ttu-id="dcb28-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dcb28-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcb28-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb28-119">Request headers</span></span>
| <span data-ttu-id="dcb28-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dcb28-120">Name</span></span>      |<span data-ttu-id="dcb28-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcb28-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcb28-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcb28-122">Authorization</span></span>  | <span data-ttu-id="dcb28-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcb28-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcb28-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dcb28-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dcb28-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dcb28-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcb28-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb28-128">Request body</span></span>
<span data-ttu-id="dcb28-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcb28-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcb28-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb28-130">Response</span></span>

<span data-ttu-id="dcb28-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcb28-131">If successful, this method returns a `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dcb28-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcb28-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcb28-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb28-133">Request</span></span>
<span data-ttu-id="dcb28-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcb28-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeborder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
```
##### <a name="response"></a><span data-ttu-id="dcb28-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb28-135">Response</span></span>
<span data-ttu-id="dcb28-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcb28-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dcb28-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dcb28-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dcb28-140">Basic</span><span class="sxs-lookup"><span data-stu-id="dcb28-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rangeborder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcb28-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcb28-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rangeborder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeborder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeborder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
