---
title: 'Table: clearFilters'
description: Limpa todos os filtros aplicados à tabela no momento.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 578857dad613289f4a3b49858d5085dbdac72fab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092990"
---
# <a name="table-clearfilters"></a><span data-ttu-id="3d346-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="3d346-103">Table: clearFilters</span></span>

<span data-ttu-id="3d346-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d346-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d346-105">Limpa todos os filtros aplicados à tabela no momento.</span><span class="sxs-lookup"><span data-stu-id="3d346-105">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d346-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d346-106">Permissions</span></span>
<span data-ttu-id="3d346-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d346-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d346-109">Permission type</span></span>      | <span data-ttu-id="3d346-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d346-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d346-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d346-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d346-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d346-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d346-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d346-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d346-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d346-115">Application</span></span> | <span data-ttu-id="3d346-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d346-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d346-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d346-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="3d346-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d346-118">Request headers</span></span>
| <span data-ttu-id="3d346-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3d346-119">Name</span></span>       | <span data-ttu-id="3d346-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d346-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d346-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d346-121">Authorization</span></span>  | <span data-ttu-id="3d346-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d346-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d346-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d346-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d346-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d346-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d346-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d346-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3d346-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d346-128">Response</span></span>

<span data-ttu-id="3d346-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d346-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d346-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d346-131">Example</span></span>
<span data-ttu-id="3d346-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3d346-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3d346-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d346-133">Request</span></span>
<span data-ttu-id="3d346-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d346-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d346-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d346-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="c"></a>[<span data-ttu-id="3d346-136">C#</span><span class="sxs-lookup"><span data-stu-id="3d346-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d346-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d346-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d346-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d346-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3d346-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d346-139">Response</span></span>
<span data-ttu-id="3d346-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d346-140">Here is an example of the response.</span></span> 
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


