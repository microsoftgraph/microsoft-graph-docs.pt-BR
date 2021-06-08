---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 6ac9fac0f389efefadeaec3a30eba0b58d851aca
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786983"
---
# <a name="filter-clear"></a><span data-ttu-id="443ca-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="443ca-103">Filter: clear</span></span>

<span data-ttu-id="443ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="443ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="443ca-105">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="443ca-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="443ca-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="443ca-106">Permissions</span></span>
<span data-ttu-id="443ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="443ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="443ca-109">Permission type</span></span>      | <span data-ttu-id="443ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="443ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="443ca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="443ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="443ca-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="443ca-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="443ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="443ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="443ca-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="443ca-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="443ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="443ca-115">Application</span></span> | <span data-ttu-id="443ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="443ca-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="443ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="443ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="443ca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="443ca-118">Request headers</span></span>
| <span data-ttu-id="443ca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="443ca-119">Name</span></span>       | <span data-ttu-id="443ca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="443ca-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="443ca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="443ca-121">Authorization</span></span>  | <span data-ttu-id="443ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="443ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="443ca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="443ca-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="443ca-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="443ca-125">Response</span></span>

<span data-ttu-id="443ca-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="443ca-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443ca-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="443ca-128">Example</span></span>
<span data-ttu-id="443ca-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="443ca-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="443ca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="443ca-130">Request</span></span>
<span data-ttu-id="443ca-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="443ca-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="443ca-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="443ca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="443ca-133">C#</span><span class="sxs-lookup"><span data-stu-id="443ca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="443ca-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="443ca-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="443ca-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="443ca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="443ca-136">Java</span><span class="sxs-lookup"><span data-stu-id="443ca-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="443ca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="443ca-137">Response</span></span>
<span data-ttu-id="443ca-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="443ca-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


