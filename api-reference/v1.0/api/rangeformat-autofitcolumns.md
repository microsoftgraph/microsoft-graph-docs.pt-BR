---
title: 'RangeFormat: autofitColumns'
description: Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 822d6e56839eaa7c86d99ff6ff3310ff6c0749b7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459787"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="65c2f-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="65c2f-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="65c2f-104">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="65c2f-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="65c2f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="65c2f-105">Permissions</span></span>
<span data-ttu-id="65c2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65c2f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65c2f-108">Permission type</span></span>      | <span data-ttu-id="65c2f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65c2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65c2f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65c2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65c2f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65c2f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="65c2f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65c2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65c2f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65c2f-113">Not supported.</span></span>    |
|<span data-ttu-id="65c2f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65c2f-114">Application</span></span> | <span data-ttu-id="65c2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65c2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65c2f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65c2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="65c2f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65c2f-117">Request headers</span></span>
| <span data-ttu-id="65c2f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="65c2f-118">Name</span></span>       | <span data-ttu-id="65c2f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="65c2f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65c2f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="65c2f-120">Authorization</span></span>  | <span data-ttu-id="65c2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65c2f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65c2f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="65c2f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="65c2f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="65c2f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65c2f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65c2f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="65c2f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="65c2f-127">Response</span></span>

<span data-ttu-id="65c2f-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65c2f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65c2f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65c2f-130">Example</span></span>
<span data-ttu-id="65c2f-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="65c2f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="65c2f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65c2f-132">Request</span></span>
<span data-ttu-id="65c2f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65c2f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65c2f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="65c2f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65c2f-135">C#</span><span class="sxs-lookup"><span data-stu-id="65c2f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65c2f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="65c2f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65c2f-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="65c2f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65c2f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="65c2f-138">Response</span></span>
<span data-ttu-id="65c2f-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65c2f-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
