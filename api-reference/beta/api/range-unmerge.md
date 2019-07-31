---
title: 'Range: unmerge'
description: Desfaz a mesclagem das células do intervalo em células separadas.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 70715a6bd73c70e25fc1da3c3bf1815f0ef97c90
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988472"
---
# <a name="range-unmerge"></a><span data-ttu-id="1706b-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="1706b-103">Range: unmerge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1706b-104">Desfaz a mesclagem das células do intervalo em células separadas.</span><span class="sxs-lookup"><span data-stu-id="1706b-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="1706b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1706b-105">Permissions</span></span>
<span data-ttu-id="1706b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1706b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1706b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1706b-108">Permission type</span></span>      | <span data-ttu-id="1706b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1706b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1706b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1706b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1706b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1706b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1706b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1706b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1706b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1706b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1706b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1706b-114">Application</span></span> | <span data-ttu-id="1706b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1706b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1706b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1706b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="1706b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1706b-117">Request headers</span></span>
| <span data-ttu-id="1706b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1706b-118">Name</span></span>       | <span data-ttu-id="1706b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1706b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1706b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1706b-120">Authorization</span></span>  | <span data-ttu-id="1706b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1706b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1706b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1706b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1706b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1706b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1706b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1706b-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1706b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1706b-127">Response</span></span>

<span data-ttu-id="1706b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1706b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1706b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1706b-130">Example</span></span>
<span data-ttu-id="1706b-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1706b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1706b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1706b-132">Request</span></span>
<span data-ttu-id="1706b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1706b-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1706b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1706b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1706b-135">C#</span><span class="sxs-lookup"><span data-stu-id="1706b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1706b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1706b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1706b-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1706b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1706b-138">Java</span><span class="sxs-lookup"><span data-stu-id="1706b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-unmerge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1706b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1706b-139">Response</span></span>
<span data-ttu-id="1706b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1706b-140">Here is an example of the response.</span></span> 
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
