---
title: Criar RangeBorder
description: Use essa API para criar uma nova RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 74ec5c2c9f620c6444ffd32508b719f7026f38a9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263606"
---
# <a name="create-rangeborder"></a><span data-ttu-id="d1fe9-103">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d1fe9-103">Create RangeBorder</span></span>

<span data-ttu-id="d1fe9-104">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1fe9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1fe9-105">Permissions</span></span>
<span data-ttu-id="d1fe9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1fe9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1fe9-108">Permission type</span></span>      | <span data-ttu-id="d1fe9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1fe9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1fe9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1fe9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d1fe9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1fe9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1fe9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1fe9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1fe9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-113">Not supported.</span></span>    |
|<span data-ttu-id="d1fe9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1fe9-114">Application</span></span> | <span data-ttu-id="d1fe9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1fe9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1fe9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="d1fe9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1fe9-117">Request headers</span></span>
| <span data-ttu-id="d1fe9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d1fe9-118">Name</span></span>       | <span data-ttu-id="d1fe9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1fe9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1fe9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1fe9-120">Authorization</span></span>  | <span data-ttu-id="d1fe9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1fe9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d1fe9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d1fe9-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1fe9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1fe9-126">Request body</span></span>
<span data-ttu-id="d1fe9-127">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookRangeBorder](../resources/rangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="d1fe9-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d1fe9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1fe9-128">Response</span></span>

<span data-ttu-id="d1fe9-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1fe9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1fe9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1fe9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1fe9-131">Request</span></span>
<span data-ttu-id="d1fe9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
<span data-ttu-id="d1fe9-133">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookRangeBorder](../resources/rangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="d1fe9-133">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d1fe9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1fe9-134">Response</span></span>
<span data-ttu-id="d1fe9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1fe9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1fe9-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d1fe9-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1fe9-139">C#</span><span class="sxs-lookup"><span data-stu-id="d1fe9-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1fe9-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1fe9-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d1fe9-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d1fe9-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
