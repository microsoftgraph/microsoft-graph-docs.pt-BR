---
title: 'Range: merge'
description: Mescla as células do intervalo em uma região da planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 54ff258a170133fe1c4a8afef244e6af300e39db
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455592"
---
# <a name="range-merge"></a><span data-ttu-id="25921-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="25921-103">Range: merge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25921-104">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="25921-104">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="25921-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="25921-105">Permissions</span></span>
<span data-ttu-id="25921-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25921-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25921-108">Permission type</span></span>      | <span data-ttu-id="25921-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25921-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25921-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25921-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25921-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25921-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="25921-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25921-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25921-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25921-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="25921-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25921-114">Application</span></span> | <span data-ttu-id="25921-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25921-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25921-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25921-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="25921-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25921-117">Request headers</span></span>
| <span data-ttu-id="25921-118">Nome</span><span class="sxs-lookup"><span data-stu-id="25921-118">Name</span></span>       | <span data-ttu-id="25921-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="25921-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="25921-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="25921-120">Authorization</span></span>  | <span data-ttu-id="25921-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25921-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25921-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="25921-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="25921-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="25921-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25921-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25921-126">Request body</span></span>
<span data-ttu-id="25921-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25921-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="25921-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="25921-128">Parameter</span></span>    | <span data-ttu-id="25921-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="25921-129">Type</span></span>   |<span data-ttu-id="25921-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="25921-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25921-131">across</span><span class="sxs-lookup"><span data-stu-id="25921-131">across</span></span>|<span data-ttu-id="25921-132">booliano</span><span class="sxs-lookup"><span data-stu-id="25921-132">boolean</span></span>|<span data-ttu-id="25921-p104">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="25921-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="25921-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="25921-136">Response</span></span>

<span data-ttu-id="25921-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25921-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25921-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25921-139">Example</span></span>
<span data-ttu-id="25921-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="25921-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="25921-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25921-141">Request</span></span>
<span data-ttu-id="25921-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25921-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25921-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="25921-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25921-144">C#</span><span class="sxs-lookup"><span data-stu-id="25921-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-merge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25921-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="25921-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-merge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25921-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="25921-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-merge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25921-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="25921-147">Response</span></span>
<span data-ttu-id="25921-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25921-148">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
