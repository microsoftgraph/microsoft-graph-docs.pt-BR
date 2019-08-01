---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: dc4919480ab7a4112ff98c3290ffb1c74bd49bf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002766"
---
# <a name="filter-clear"></a><span data-ttu-id="1d55e-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="1d55e-103">Filter: clear</span></span>

<span data-ttu-id="1d55e-104">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="1d55e-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d55e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d55e-105">Permissions</span></span>
<span data-ttu-id="1d55e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d55e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d55e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d55e-108">Permission type</span></span>      | <span data-ttu-id="1d55e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d55e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d55e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d55e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d55e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d55e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d55e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d55e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d55e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d55e-113">Not supported.</span></span>    |
|<span data-ttu-id="1d55e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d55e-114">Application</span></span> | <span data-ttu-id="1d55e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d55e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d55e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d55e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="1d55e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d55e-117">Request headers</span></span>
| <span data-ttu-id="1d55e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1d55e-118">Name</span></span>       | <span data-ttu-id="1d55e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d55e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d55e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d55e-120">Authorization</span></span>  | <span data-ttu-id="1d55e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d55e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d55e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d55e-123">Request body</span></span>
<span data-ttu-id="1d55e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d55e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d55e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d55e-125">Response</span></span>

<span data-ttu-id="1d55e-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d55e-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d55e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d55e-128">Example</span></span>
<span data-ttu-id="1d55e-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1d55e-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d55e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d55e-130">Request</span></span>
<span data-ttu-id="1d55e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d55e-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1d55e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d55e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1d55e-133">C#</span><span class="sxs-lookup"><span data-stu-id="1d55e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d55e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1d55e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1d55e-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1d55e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1d55e-136">Java</span><span class="sxs-lookup"><span data-stu-id="1d55e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d55e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d55e-137">Response</span></span>
<span data-ttu-id="1d55e-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d55e-138">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
