---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
ms.openlocfilehash: 9b796965c14a096a91e4c7dd416a0830bce8ba26
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614606"
---
# <a name="filter-clear"></a><span data-ttu-id="bf5a6-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="bf5a6-103">Filter: clear</span></span>

<span data-ttu-id="bf5a6-104">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf5a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf5a6-105">Permissions</span></span>
<span data-ttu-id="bf5a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf5a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf5a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf5a6-108">Permission type</span></span>      | <span data-ttu-id="bf5a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf5a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf5a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf5a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bf5a6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf5a6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf5a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf5a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf5a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-113">Not supported.</span></span>    |
|<span data-ttu-id="bf5a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf5a6-114">Application</span></span> | <span data-ttu-id="bf5a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf5a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf5a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="bf5a6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf5a6-117">Request headers</span></span>
| <span data-ttu-id="bf5a6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bf5a6-118">Name</span></span>       | <span data-ttu-id="bf5a6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf5a6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf5a6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf5a6-120">Authorization</span></span>  | <span data-ttu-id="bf5a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf5a6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf5a6-123">Request body</span></span>
<span data-ttu-id="bf5a6-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf5a6-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf5a6-125">Response</span></span>

<span data-ttu-id="bf5a6-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf5a6-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf5a6-128">Example</span></span>
<span data-ttu-id="bf5a6-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf5a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf5a6-130">Request</span></span>
<span data-ttu-id="bf5a6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="bf5a6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf5a6-132">Response</span></span>
<span data-ttu-id="bf5a6-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf5a6-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf5a6-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bf5a6-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf5a6-135">Basic</span><span class="sxs-lookup"><span data-stu-id="bf5a6-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/filter_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf5a6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf5a6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/filter_clear-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/filter-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
