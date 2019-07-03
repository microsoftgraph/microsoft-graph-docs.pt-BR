---
title: 'Table: clearFilters'
description: Limpa todos os filtros aplicados à tabela no momento.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 948621a81d105181572c2c7372167de90a4051c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456957"
---
# <a name="table-clearfilters"></a><span data-ttu-id="413ff-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="413ff-103">Table: clearFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="413ff-104">Limpa todos os filtros aplicados à tabela no momento.</span><span class="sxs-lookup"><span data-stu-id="413ff-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="413ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="413ff-105">Permissions</span></span>
<span data-ttu-id="413ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="413ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="413ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="413ff-108">Permission type</span></span>      | <span data-ttu-id="413ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="413ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="413ff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="413ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="413ff-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="413ff-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="413ff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="413ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="413ff-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="413ff-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="413ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="413ff-114">Application</span></span> | <span data-ttu-id="413ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="413ff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="413ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="413ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="413ff-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="413ff-117">Request headers</span></span>
| <span data-ttu-id="413ff-118">Nome</span><span class="sxs-lookup"><span data-stu-id="413ff-118">Name</span></span>       | <span data-ttu-id="413ff-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="413ff-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="413ff-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="413ff-120">Authorization</span></span>  | <span data-ttu-id="413ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="413ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="413ff-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="413ff-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="413ff-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="413ff-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="413ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="413ff-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="413ff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="413ff-127">Response</span></span>

<span data-ttu-id="413ff-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="413ff-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="413ff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="413ff-130">Example</span></span>
<span data-ttu-id="413ff-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="413ff-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="413ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="413ff-132">Request</span></span>
<span data-ttu-id="413ff-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="413ff-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="413ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="413ff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="413ff-135">C#</span><span class="sxs-lookup"><span data-stu-id="413ff-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="413ff-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="413ff-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="413ff-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="413ff-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="413ff-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="413ff-138">Response</span></span>
<span data-ttu-id="413ff-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="413ff-139">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
