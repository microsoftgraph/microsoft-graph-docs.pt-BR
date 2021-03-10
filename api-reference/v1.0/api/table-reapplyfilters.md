---
title: 'Table: reapplyFilters'
description: Aplica novamente todos os filtros à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0b070a1f355273eaccc42d06eb29c64f62e7de6a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577160"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="5d439-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="5d439-103">Table: reapplyFilters</span></span>

<span data-ttu-id="5d439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d439-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d439-105">Aplica novamente todos os filtros à tabela.</span><span class="sxs-lookup"><span data-stu-id="5d439-105">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d439-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d439-106">Permissions</span></span>
<span data-ttu-id="5d439-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d439-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d439-109">Permission type</span></span>      | <span data-ttu-id="5d439-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d439-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d439-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d439-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d439-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d439-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d439-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d439-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d439-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d439-114">Not supported.</span></span>    |
|<span data-ttu-id="5d439-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d439-115">Application</span></span> | <span data-ttu-id="5d439-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d439-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d439-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d439-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/reapplyFilters
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="5d439-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d439-118">Request headers</span></span>
| <span data-ttu-id="5d439-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5d439-119">Name</span></span>       | <span data-ttu-id="5d439-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d439-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d439-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d439-121">Authorization</span></span>  | <span data-ttu-id="5d439-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d439-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d439-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5d439-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5d439-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d439-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d439-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d439-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5d439-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d439-128">Response</span></span>

<span data-ttu-id="5d439-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d439-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d439-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d439-131">Example</span></span>
<span data-ttu-id="5d439-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5d439-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d439-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d439-133">Request</span></span>
<span data-ttu-id="5d439-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d439-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d439-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d439-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```
# <a name="c"></a>[<span data-ttu-id="5d439-136">C#</span><span class="sxs-lookup"><span data-stu-id="5d439-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-reapplyfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d439-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d439-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-reapplyfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d439-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d439-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-reapplyfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d439-139">Java</span><span class="sxs-lookup"><span data-stu-id="5d439-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-reapplyfilters-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d439-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d439-140">Response</span></span>
<span data-ttu-id="5d439-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d439-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

