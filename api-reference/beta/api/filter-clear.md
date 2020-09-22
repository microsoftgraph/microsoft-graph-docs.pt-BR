---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 73f4071bd9a5be480afb2a0049763a66b7026e44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006682"
---
# <a name="filter-clear"></a><span data-ttu-id="84995-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="84995-103">Filter: clear</span></span>

<span data-ttu-id="84995-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="84995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84995-105">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="84995-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="84995-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84995-106">Permissions</span></span>
<span data-ttu-id="84995-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84995-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84995-109">Permission type</span></span>      | <span data-ttu-id="84995-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84995-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84995-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84995-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84995-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84995-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84995-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84995-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84995-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84995-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84995-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84995-115">Application</span></span> | <span data-ttu-id="84995-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84995-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84995-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84995-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="84995-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84995-118">Request headers</span></span>
| <span data-ttu-id="84995-119">Nome</span><span class="sxs-lookup"><span data-stu-id="84995-119">Name</span></span>       | <span data-ttu-id="84995-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="84995-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="84995-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="84995-121">Authorization</span></span>  | <span data-ttu-id="84995-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84995-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84995-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84995-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="84995-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="84995-125">Response</span></span>

<span data-ttu-id="84995-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84995-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84995-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84995-128">Example</span></span>
<span data-ttu-id="84995-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="84995-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84995-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84995-130">Request</span></span>
<span data-ttu-id="84995-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84995-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84995-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="84995-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="84995-133">C#</span><span class="sxs-lookup"><span data-stu-id="84995-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84995-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84995-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84995-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84995-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="84995-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="84995-136">Response</span></span>
<span data-ttu-id="84995-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84995-137">Here is an example of the response.</span></span>
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


