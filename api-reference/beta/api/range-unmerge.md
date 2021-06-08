---
title: 'Range: unmerge'
description: Desfaz a mesclagem das células do intervalo em células separadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d5958121e761c17f5acb6cebebe154eac4cee66c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785897"
---
# <a name="range-unmerge"></a><span data-ttu-id="2ceff-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="2ceff-103">Range: unmerge</span></span>

<span data-ttu-id="2ceff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ceff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ceff-105">Desfaz a mesclagem das células do intervalo em células separadas.</span><span class="sxs-lookup"><span data-stu-id="2ceff-105">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ceff-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2ceff-106">Permissions</span></span>
<span data-ttu-id="2ceff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ceff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ceff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ceff-109">Permission type</span></span>      | <span data-ttu-id="2ceff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ceff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ceff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ceff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ceff-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ceff-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ceff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ceff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ceff-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ceff-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ceff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ceff-115">Application</span></span> | <span data-ttu-id="2ceff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ceff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ceff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ceff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/unmerge
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/unmerge
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/unmerge
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="2ceff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ceff-118">Request headers</span></span>
| <span data-ttu-id="2ceff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ceff-119">Name</span></span>       | <span data-ttu-id="2ceff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ceff-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ceff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ceff-121">Authorization</span></span>  | <span data-ttu-id="2ceff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ceff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ceff-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ceff-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ceff-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2ceff-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ceff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ceff-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2ceff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ceff-128">Response</span></span>

<span data-ttu-id="2ceff-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ceff-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ceff-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ceff-131">Example</span></span>
<span data-ttu-id="2ceff-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2ceff-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ceff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ceff-133">Request</span></span>
<span data-ttu-id="2ceff-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ceff-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ceff-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ceff-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="c"></a>[<span data-ttu-id="2ceff-136">C#</span><span class="sxs-lookup"><span data-stu-id="2ceff-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ceff-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ceff-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ceff-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ceff-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ceff-139">Java</span><span class="sxs-lookup"><span data-stu-id="2ceff-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-unmerge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ceff-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ceff-140">Response</span></span>
<span data-ttu-id="2ceff-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ceff-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


