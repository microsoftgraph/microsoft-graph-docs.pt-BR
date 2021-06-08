---
title: 'Chart: delete'
description: Exclui o objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 15fba815d2f49d3fa13f8c99569f2a31de0ee742
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786205"
---
# <a name="chart-delete"></a><span data-ttu-id="813ae-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="813ae-103">Chart: delete</span></span>

<span data-ttu-id="813ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="813ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="813ae-105">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="813ae-105">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="813ae-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="813ae-106">Permissions</span></span>
<span data-ttu-id="813ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="813ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="813ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="813ae-109">Permission type</span></span>      | <span data-ttu-id="813ae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="813ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="813ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="813ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="813ae-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="813ae-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="813ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="813ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="813ae-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="813ae-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="813ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="813ae-115">Application</span></span> | <span data-ttu-id="813ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="813ae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="813ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="813ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}
```
## <a name="request-headers"></a><span data-ttu-id="813ae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="813ae-118">Request headers</span></span>
| <span data-ttu-id="813ae-119">Nome</span><span class="sxs-lookup"><span data-stu-id="813ae-119">Name</span></span>       | <span data-ttu-id="813ae-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="813ae-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="813ae-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="813ae-121">Authorization</span></span>  | <span data-ttu-id="813ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="813ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="813ae-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="813ae-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="813ae-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="813ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="813ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="813ae-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="813ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="813ae-128">Response</span></span>

<span data-ttu-id="813ae-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="813ae-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="813ae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="813ae-131">Example</span></span>
<span data-ttu-id="813ae-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="813ae-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="813ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="813ae-133">Request</span></span>
<span data-ttu-id="813ae-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="813ae-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="813ae-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="813ae-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```
# <a name="c"></a>[<span data-ttu-id="813ae-136">C#</span><span class="sxs-lookup"><span data-stu-id="813ae-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="813ae-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="813ae-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="813ae-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="813ae-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="813ae-139">Java</span><span class="sxs-lookup"><span data-stu-id="813ae-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="813ae-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="813ae-140">Response</span></span>
<span data-ttu-id="813ae-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="813ae-141">Here is an example of the response.</span></span> 
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
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


