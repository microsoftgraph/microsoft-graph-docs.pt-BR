---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
ms.openlocfilehash: 2bc1d1f607f062ca7566189d184f37bc74ab09df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440859"
---
# <a name="filter-clear"></a><span data-ttu-id="22d1c-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="22d1c-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d1c-104">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="22d1c-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="22d1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="22d1c-105">Permissions</span></span>
<span data-ttu-id="22d1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22d1c-108">Permission type</span></span>      | <span data-ttu-id="22d1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22d1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22d1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22d1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="22d1c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22d1c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22d1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22d1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22d1c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22d1c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22d1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22d1c-114">Application</span></span> | <span data-ttu-id="22d1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22d1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22d1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22d1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="22d1c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22d1c-117">Request headers</span></span>
| <span data-ttu-id="22d1c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="22d1c-118">Name</span></span>       | <span data-ttu-id="22d1c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="22d1c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="22d1c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="22d1c-120">Authorization</span></span>  | <span data-ttu-id="22d1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22d1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22d1c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22d1c-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="22d1c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="22d1c-124">Response</span></span>

<span data-ttu-id="22d1c-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22d1c-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d1c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22d1c-127">Example</span></span>
<span data-ttu-id="22d1c-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="22d1c-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="22d1c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22d1c-129">Request</span></span>
<span data-ttu-id="22d1c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22d1c-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22d1c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="22d1c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22d1c-132">C#</span><span class="sxs-lookup"><span data-stu-id="22d1c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22d1c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="22d1c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22d1c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="22d1c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="22d1c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="22d1c-135">Response</span></span>
<span data-ttu-id="22d1c-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22d1c-136">Here is an example of the response.</span></span> 
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
