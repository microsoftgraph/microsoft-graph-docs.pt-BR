---
title: 'Worksheet: delete'
description: Exclui a planilha da pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d2cfde98485c1f17fa5fe6f08ed8e48e85f855f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771229"
---
# <a name="worksheet-delete"></a><span data-ttu-id="3cc0b-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="3cc0b-103">Worksheet: delete</span></span>

<span data-ttu-id="3cc0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cc0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cc0b-105">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="3cc0b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3cc0b-106">Permissions</span></span>
<span data-ttu-id="3cc0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cc0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cc0b-109">Permission type</span></span>      | <span data-ttu-id="3cc0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cc0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cc0b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cc0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3cc0b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cc0b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3cc0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cc0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cc0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-114">Not supported.</span></span>    |
|<span data-ttu-id="3cc0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cc0b-115">Application</span></span> | <span data-ttu-id="3cc0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cc0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc0b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="3cc0b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc0b-118">Request headers</span></span>
| <span data-ttu-id="3cc0b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3cc0b-119">Name</span></span>       | <span data-ttu-id="3cc0b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc0b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3cc0b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cc0b-121">Authorization</span></span>  | <span data-ttu-id="3cc0b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3cc0b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3cc0b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3cc0b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cc0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc0b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3cc0b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc0b-128">Response</span></span>

<span data-ttu-id="3cc0b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cc0b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cc0b-131">Example</span></span>
<span data-ttu-id="3cc0b-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3cc0b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc0b-133">Request</span></span>
<span data-ttu-id="3cc0b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cc0b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc0b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="3cc0b-136">C#</span><span class="sxs-lookup"><span data-stu-id="3cc0b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cc0b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cc0b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cc0b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cc0b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cc0b-139">Java</span><span class="sxs-lookup"><span data-stu-id="3cc0b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cc0b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc0b-140">Response</span></span>
<span data-ttu-id="3cc0b-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-141">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

