---
title: 'RangeFormat: autofitColumns'
description: Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1bd731ce30ce4fcd87d2bfc542208f8252774ddf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412030"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="08440-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="08440-103">RangeFormat: autofitColumns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08440-104">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="08440-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="08440-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08440-105">Permissions</span></span>
<span data-ttu-id="08440-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08440-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08440-108">Permission type</span></span>      | <span data-ttu-id="08440-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08440-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08440-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08440-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08440-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08440-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08440-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08440-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08440-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08440-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08440-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08440-114">Application</span></span> | <span data-ttu-id="08440-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08440-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08440-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08440-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="08440-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08440-117">Request headers</span></span>
| <span data-ttu-id="08440-118">Nome</span><span class="sxs-lookup"><span data-stu-id="08440-118">Name</span></span>       | <span data-ttu-id="08440-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="08440-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08440-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="08440-120">Authorization</span></span>  | <span data-ttu-id="08440-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08440-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08440-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08440-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="08440-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="08440-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08440-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08440-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="08440-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="08440-127">Response</span></span>

<span data-ttu-id="08440-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08440-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08440-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08440-130">Example</span></span>
<span data-ttu-id="08440-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="08440-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08440-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08440-132">Request</span></span>
<span data-ttu-id="08440-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08440-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08440-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="08440-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08440-135">C#</span><span class="sxs-lookup"><span data-stu-id="08440-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08440-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08440-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08440-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="08440-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08440-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="08440-138">Response</span></span>
<span data-ttu-id="08440-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08440-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
