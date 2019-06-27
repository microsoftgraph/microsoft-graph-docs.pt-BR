---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0bd18479f62b88d98064380e07a32d9c36c2ae96
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265545"
---
# <a name="range-lastrow"></a><span data-ttu-id="de6eb-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="de6eb-103">Range: LastRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6eb-p101">Obtém a última linha do intervalo. Por exemplo, a última linha de "B2:D5" é "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="de6eb-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="de6eb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de6eb-106">Permissions</span></span>
<span data-ttu-id="de6eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6eb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de6eb-109">Permission type</span></span>      | <span data-ttu-id="de6eb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de6eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6eb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de6eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de6eb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6eb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de6eb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de6eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6eb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6eb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de6eb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de6eb-115">Application</span></span> | <span data-ttu-id="de6eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de6eb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de6eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de6eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="de6eb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de6eb-118">Request headers</span></span>
| <span data-ttu-id="de6eb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="de6eb-119">Name</span></span>       | <span data-ttu-id="de6eb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="de6eb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de6eb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="de6eb-121">Authorization</span></span>  | <span data-ttu-id="de6eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6eb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de6eb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="de6eb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="de6eb-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="de6eb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de6eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de6eb-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="de6eb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="de6eb-128">Response</span></span>

<span data-ttu-id="de6eb-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de6eb-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de6eb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de6eb-130">Example</span></span>
<span data-ttu-id="de6eb-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="de6eb-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de6eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de6eb-132">Request</span></span>
<span data-ttu-id="de6eb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de6eb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="de6eb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="de6eb-134">Response</span></span>
<span data-ttu-id="de6eb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de6eb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="de6eb-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="de6eb-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de6eb-139">C#</span><span class="sxs-lookup"><span data-stu-id="de6eb-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_lastrow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6eb-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6eb-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_lastrow-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6eb-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6eb-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_lastrow-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
