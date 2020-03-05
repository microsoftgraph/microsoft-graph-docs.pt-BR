---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 1f2a766167a629b976caadd7698884c794f2be68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421645"
---
# <a name="filter-clear"></a><span data-ttu-id="7137e-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="7137e-103">Filter: clear</span></span>

<span data-ttu-id="7137e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7137e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7137e-105">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="7137e-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="7137e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7137e-106">Permissions</span></span>
<span data-ttu-id="7137e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7137e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7137e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7137e-109">Permission type</span></span>      | <span data-ttu-id="7137e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7137e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7137e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7137e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7137e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7137e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7137e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7137e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7137e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7137e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7137e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7137e-115">Application</span></span> | <span data-ttu-id="7137e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7137e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7137e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7137e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="7137e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7137e-118">Request headers</span></span>
| <span data-ttu-id="7137e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7137e-119">Name</span></span>       | <span data-ttu-id="7137e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7137e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7137e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7137e-121">Authorization</span></span>  | <span data-ttu-id="7137e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7137e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7137e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7137e-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7137e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7137e-125">Response</span></span>

<span data-ttu-id="7137e-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7137e-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7137e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7137e-128">Example</span></span>
<span data-ttu-id="7137e-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7137e-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7137e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7137e-130">Request</span></span>
<span data-ttu-id="7137e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7137e-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7137e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7137e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="7137e-133">C#</span><span class="sxs-lookup"><span data-stu-id="7137e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7137e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7137e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7137e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7137e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7137e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7137e-136">Response</span></span>
<span data-ttu-id="7137e-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7137e-137">Here is an example of the response.</span></span> 
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
