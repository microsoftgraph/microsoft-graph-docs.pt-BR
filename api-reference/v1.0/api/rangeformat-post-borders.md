---
title: Criar RangeBorder
description: Use essa API para criar uma nova RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 613cda9d863976c28c2d21847a6f52692e512f67
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607427"
---
# <a name="create-rangeborder"></a><span data-ttu-id="73fc1-103">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="73fc1-103">Create RangeBorder</span></span>

<span data-ttu-id="73fc1-104">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="73fc1-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="73fc1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="73fc1-105">Permissions</span></span>
<span data-ttu-id="73fc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73fc1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73fc1-108">Permission type</span></span>      | <span data-ttu-id="73fc1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73fc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73fc1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73fc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73fc1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73fc1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73fc1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73fc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73fc1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73fc1-113">Not supported.</span></span>    |
|<span data-ttu-id="73fc1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73fc1-114">Application</span></span> | <span data-ttu-id="73fc1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73fc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73fc1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73fc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="73fc1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73fc1-117">Request headers</span></span>
| <span data-ttu-id="73fc1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="73fc1-118">Name</span></span>       | <span data-ttu-id="73fc1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="73fc1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73fc1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="73fc1-120">Authorization</span></span>  | <span data-ttu-id="73fc1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73fc1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73fc1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="73fc1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="73fc1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="73fc1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73fc1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73fc1-126">Request body</span></span>
<span data-ttu-id="73fc1-127">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookRangeBorder](../resources/rangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="73fc1-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="73fc1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="73fc1-128">Response</span></span>

<span data-ttu-id="73fc1-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73fc1-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73fc1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73fc1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73fc1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73fc1-131">Request</span></span>
<span data-ttu-id="73fc1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73fc1-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="73fc1-133">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookRangeBorder](../resources/rangeborder.md) .</span><span class="sxs-lookup"><span data-stu-id="73fc1-133">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="73fc1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="73fc1-134">Response</span></span>
<span data-ttu-id="73fc1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73fc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="73fc1-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="73fc1-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="73fc1-139">Basic</span><span class="sxs-lookup"><span data-stu-id="73fc1-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73fc1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73fc1-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
