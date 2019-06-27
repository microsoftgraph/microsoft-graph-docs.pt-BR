---
title: 'Range: EntireColumn'
description: Obtém um objeto que representa toda a coluna do intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fe3f73aa2cb4a0a955ff7686ca3cdef189c3af46
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276038"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="36d72-103">Range: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="36d72-103">Range: EntireColumn</span></span>

<span data-ttu-id="36d72-104">Obtém um objeto que representa toda a coluna do intervalo.</span><span class="sxs-lookup"><span data-stu-id="36d72-104">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="36d72-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="36d72-105">Permissions</span></span>
<span data-ttu-id="36d72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36d72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36d72-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36d72-108">Permission type</span></span>      | <span data-ttu-id="36d72-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36d72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36d72-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36d72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36d72-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36d72-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36d72-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36d72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36d72-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36d72-113">Not supported.</span></span>    |
|<span data-ttu-id="36d72-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36d72-114">Application</span></span> | <span data-ttu-id="36d72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36d72-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36d72-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36d72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireColumn

```
## <a name="request-headers"></a><span data-ttu-id="36d72-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36d72-117">Request headers</span></span>
| <span data-ttu-id="36d72-118">Nome</span><span class="sxs-lookup"><span data-stu-id="36d72-118">Name</span></span>       | <span data-ttu-id="36d72-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="36d72-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36d72-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="36d72-120">Authorization</span></span>  | <span data-ttu-id="36d72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36d72-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36d72-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36d72-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="36d72-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="36d72-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36d72-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36d72-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="36d72-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="36d72-127">Response</span></span>

<span data-ttu-id="36d72-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36d72-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d72-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36d72-129">Example</span></span>
<span data-ttu-id="36d72-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="36d72-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36d72-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36d72-131">Request</span></span>
<span data-ttu-id="36d72-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36d72-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireColumn
```

##### <a name="response"></a><span data-ttu-id="36d72-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="36d72-133">Response</span></span>
<span data-ttu-id="36d72-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36d72-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="36d72-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="36d72-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="36d72-138">C#</span><span class="sxs-lookup"><span data-stu-id="36d72-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_entirecolumn-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36d72-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="36d72-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_entirecolumn-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="36d72-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="36d72-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_entirecolumn-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-entirecolumn.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/range-entirecolumn.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-entirecolumn.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
