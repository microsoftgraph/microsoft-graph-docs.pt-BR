---
title: 'RangeFormat: autofitColumns'
description: Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: bf1578efb3a4c4911ca924212cd0666e9c81f6d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263662"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="c6668-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="c6668-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="c6668-104">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="c6668-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6668-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6668-105">Permissions</span></span>
<span data-ttu-id="c6668-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6668-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6668-108">Permission type</span></span>      | <span data-ttu-id="c6668-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6668-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6668-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6668-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6668-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6668-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6668-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6668-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6668-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6668-113">Not supported.</span></span>    |
|<span data-ttu-id="c6668-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6668-114">Application</span></span> | <span data-ttu-id="c6668-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6668-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6668-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6668-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="c6668-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6668-117">Request headers</span></span>
| <span data-ttu-id="c6668-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c6668-118">Name</span></span>       | <span data-ttu-id="c6668-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6668-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6668-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6668-120">Authorization</span></span>  | <span data-ttu-id="c6668-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6668-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6668-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c6668-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6668-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c6668-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6668-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6668-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c6668-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6668-127">Response</span></span>

<span data-ttu-id="c6668-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6668-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6668-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6668-130">Example</span></span>
<span data-ttu-id="c6668-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c6668-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6668-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6668-132">Request</span></span>
<span data-ttu-id="c6668-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6668-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="c6668-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6668-134">Response</span></span>
<span data-ttu-id="c6668-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6668-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6668-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c6668-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6668-137">C#</span><span class="sxs-lookup"><span data-stu-id="c6668-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/rangeformat_autofitcolumns-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6668-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6668-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangeformat_autofitcolumns-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6668-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c6668-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/rangeformat_autofitcolumns-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-autofitcolumns.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-autofitcolumns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-autofitcolumns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
