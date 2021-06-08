---
title: 'Worksheet: delete'
description: Exclui a planilha da pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6689b65c3aea25a620692deb57a5362564422254
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786086"
---
# <a name="worksheet-delete"></a><span data-ttu-id="dbe2a-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="dbe2a-103">Worksheet: delete</span></span>

<span data-ttu-id="dbe2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbe2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbe2a-105">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbe2a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dbe2a-106">Permissions</span></span>
<span data-ttu-id="dbe2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbe2a-109">Permission type</span></span>      | <span data-ttu-id="dbe2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbe2a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbe2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbe2a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbe2a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe2a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbe2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbe2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbe2a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe2a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbe2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbe2a-115">Application</span></span> | <span data-ttu-id="dbe2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbe2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe2a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="dbe2a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe2a-118">Request headers</span></span>
| <span data-ttu-id="dbe2a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dbe2a-119">Name</span></span>       | <span data-ttu-id="dbe2a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbe2a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dbe2a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbe2a-121">Authorization</span></span>  | <span data-ttu-id="dbe2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbe2a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dbe2a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dbe2a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbe2a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe2a-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dbe2a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe2a-128">Response</span></span>

<span data-ttu-id="dbe2a-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe2a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbe2a-131">Example</span></span>
<span data-ttu-id="dbe2a-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dbe2a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe2a-133">Request</span></span>
<span data-ttu-id="dbe2a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dbe2a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe2a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="dbe2a-136">C#</span><span class="sxs-lookup"><span data-stu-id="dbe2a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbe2a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbe2a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbe2a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbe2a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dbe2a-139">Java</span><span class="sxs-lookup"><span data-stu-id="dbe2a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dbe2a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe2a-140">Response</span></span>
<span data-ttu-id="dbe2a-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-141">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


