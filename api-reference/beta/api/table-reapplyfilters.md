---
title: 'Table: reapplyFilters'
description: Aplica novamente todos os filtros à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a873e2af298ab388d3b390db7effe888ade55d41
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868815"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="94a89-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="94a89-103">Table: reapplyFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a89-104">Aplica novamente todos os filtros à tabela.</span><span class="sxs-lookup"><span data-stu-id="94a89-104">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="94a89-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a89-105">Permissions</span></span>
<span data-ttu-id="94a89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a89-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a89-108">Permission type</span></span>      | <span data-ttu-id="94a89-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a89-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94a89-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94a89-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94a89-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a89-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94a89-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94a89-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a89-114">Application</span></span> | <span data-ttu-id="94a89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a89-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a89-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="94a89-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a89-117">Request headers</span></span>
| <span data-ttu-id="94a89-118">Nome</span><span class="sxs-lookup"><span data-stu-id="94a89-118">Name</span></span>       | <span data-ttu-id="94a89-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a89-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94a89-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a89-120">Authorization</span></span>  | <span data-ttu-id="94a89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94a89-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94a89-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="94a89-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="94a89-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a89-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a89-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="94a89-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a89-127">Response</span></span>

<span data-ttu-id="94a89-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a89-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a89-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a89-130">Example</span></span>
<span data-ttu-id="94a89-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="94a89-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94a89-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a89-132">Request</span></span>
<span data-ttu-id="94a89-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a89-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94a89-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94a89-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94a89-135">C#</span><span class="sxs-lookup"><span data-stu-id="94a89-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-reapplyfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94a89-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="94a89-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-reapplyfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94a89-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="94a89-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-reapplyfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="94a89-138">Java</span><span class="sxs-lookup"><span data-stu-id="94a89-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-reapplyfilters-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94a89-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a89-139">Response</span></span>
<span data-ttu-id="94a89-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a89-140">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
