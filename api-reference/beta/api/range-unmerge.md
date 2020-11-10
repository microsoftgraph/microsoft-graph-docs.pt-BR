---
title: 'Range: unmerge'
description: Desfaz a mesclagem das células do intervalo em células separadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7c1ff8bbc7f2dc0bf8ed3d32d7beec95a27507b9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981200"
---
# <a name="range-unmerge"></a><span data-ttu-id="276ab-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="276ab-103">Range: unmerge</span></span>

<span data-ttu-id="276ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="276ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="276ab-105">Desfaz a mesclagem das células do intervalo em células separadas.</span><span class="sxs-lookup"><span data-stu-id="276ab-105">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="276ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="276ab-106">Permissions</span></span>
<span data-ttu-id="276ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="276ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="276ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="276ab-109">Permission type</span></span>      | <span data-ttu-id="276ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="276ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="276ab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="276ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="276ab-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276ab-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="276ab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="276ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276ab-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276ab-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="276ab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="276ab-115">Application</span></span> | <span data-ttu-id="276ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="276ab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="276ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="276ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="276ab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="276ab-118">Request headers</span></span>
| <span data-ttu-id="276ab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="276ab-119">Name</span></span>       | <span data-ttu-id="276ab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="276ab-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="276ab-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="276ab-121">Authorization</span></span>  | <span data-ttu-id="276ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="276ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="276ab-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="276ab-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="276ab-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="276ab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="276ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="276ab-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="276ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="276ab-128">Response</span></span>

<span data-ttu-id="276ab-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="276ab-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="276ab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="276ab-131">Example</span></span>
<span data-ttu-id="276ab-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="276ab-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="276ab-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="276ab-133">Request</span></span>
<span data-ttu-id="276ab-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="276ab-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="276ab-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="276ab-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="c"></a>[<span data-ttu-id="276ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="276ab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="276ab-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="276ab-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="276ab-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="276ab-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="276ab-139">Java</span><span class="sxs-lookup"><span data-stu-id="276ab-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-unmerge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="276ab-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="276ab-140">Response</span></span>
<span data-ttu-id="276ab-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="276ab-141">Here is an example of the response.</span></span> 
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
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


